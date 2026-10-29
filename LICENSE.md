# NILS model licence

Version 1, draft of 2026-10-29.

These terms cover the trained model files that NILS reads as model inputs (for example the post-contrast model r1: its fusion and its three image arms with their atlases), their cards, and any file we publish under this licence. They do not cover the NILS software, which is under the GNU Affero General Public License version 3, nor any data.

By downloading, copying or using the files you accept these terms. If you do not accept them, do not download or use the files.

## 1. What you may do

You may use the files for research and for the evaluation of NILS, at your own institution, on your own data. You may fine-tune or adapt them for the same purpose.

## 2. What you may not do

- Use the files, or anything derived from them, to make or support a clinical decision about a person. The models are research tools and are not certified medical devices.
- Pass the files on, re-host them, or make them available to anyone outside your institution. Point others to our download instead.
- Use the files, or anything derived from them, in a product or service, or for any commercial purpose, without our written permission.
- Try to recover from the files any information about the people whose scans they were trained on.

## 3. Derived models

A model you fine-tune or adapt from the files is under these same terms. Tell us about it if you publish results from it, and name it as derived from the NILS model it came from.

## 4. Calibration

A model's answers are certified only for the scanners and sites its card names. For any other site the model answers "not sure" until that site's own calibration exists, and a raw score it writes in test mode is for inspection, never a label.

## 5. Citation

Work that uses the files cites NILS: Chamyani N, et al. NILS post-contrast model r1 (model files). Kineuro, Karolinska Institutet, 2026. https://github.com/kineuro/nils-models. The current line is in the model's card and on the download page; once the NILS paper is published, it replaces this line.

## 6. No warranty

The files are provided as they are, without any warranty of any kind, and we are not liable for anything that follows from their use. The models were trained on pseudonymised clinical images under ethics permit 2019-02862 and its amendments; the files hold model parameters and no image or personal data.

## 7. Changes and withdrawal

We may publish new versions of the files and withdraw old ones. If we ask you to stop using a version, delete your copies of it within 30 days.

## 8. Law

Swedish law applies.

Kineuro, Karolinska Institutet, Stockholm.
