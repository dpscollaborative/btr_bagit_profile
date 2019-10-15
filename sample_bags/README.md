# Sample Bags

Test your BagIt validator against these bags. Each of the "bad" bags should fail for
the specified reasons. Each of the "good" bags should be valid.

## btr_bad_checksums.tar

* In manifest-sha512.txt, bad digest for data/netutil/listen_test.go
* In tagmanifest-sha512.txt, bad digest for manifest-sha512.txt

## btr_bad_extraneous_file.tar

* Payload file data/nsqd.dat is not in manifest-sha512.txt
* Payload-Oxum says there should be 6 files in the payload, but there are 7.
* Payload-Oxum says there should be 18242 bytes in the payload, but there are 18273

## btr_bad_missing_payload_file.tar

* File 'data/netutil/listen.go' is missing from data directory
* Payload-Oxum says there should be 6 files in the payload, but there are 5.
* Payload-Oxum says there should be 18242 bytes in the payload, but there are 17083.

## btr_bad_missing_required_tags.tar

This bag is invalid because bag-info.txt is missing the following required tags:

* Bagging-Date
* Payload-Oxum
* Source-Organization

## btr_good_sha256.tar

This bag is valid. It includes a sha256 payload manifest and a sha256 tag manifest.

## btr_good_sha512.tar

This bag is valid. It includes a sha512 payload manifest and a sha512 tag manifest.

