# Digests()
Digests hashes each segment of each key fragment 26 times and returns them. Optionally takes the SpongeFunction to use. Default is Kerl.
> **Important note:** This API is currently in Beta and is subject to change. Use of these APIs in production applications is not supported.


## Input

| Parameter       | Type | Required or Optional | Description |
|:---------------|:--------|:--------| :--------|
| key | Trits | Required | The private key from which to derive the digests from.  |
| spongeFunc | ...SpongeFunction | Optional | The optional sponge function to use.  |




## Output

| Return type     | Description |
|:---------------|:--------|
| Trits | The Trits representation of the digests. |
| error | Returned for internal errors. |




## Example

```go
func ExampleDigests() 
	key := "D9DWVXXXMGBR9BKHQMMRTQIQROKTLOZNNYHHETDLHVE9FUIBGLEVSTHMJHNHXRRYWHBLNUICBOQHVGBRDSAJZKOL9EQNXGHCETSGW9LTGJPMKD9DEFITRUDVUUSKR9BMMAABVJIKICTLEGBSDMHGGOEALGWBZCF9YCWUANXAZOZJFQARYCKNOJTCXBYEWENKABGSUQXLOM9ZNEDVZQMUPWROQVQXTHLDUKMRULEZDOW9MEXSELWIKHYTCXQNWYIRLNQWUEOBPBQZTHNMRSMNIRQ9BKDHPDGN9VRZEBXKTFCCXOETJKX9YYJDB9HGLCOHMPOXRXBBV9YDSLYPBVABTNOWKXLSTGZAA9EXHLLGWIISYOSQQKYYOXSJDXVSLHDASEXDYJTFRRHLRMKLHZESDGTDGLUNLOWIETHXWEWPDCJRGMKFMXVNPLBGRYMAXTTAILUGAFUIXGTDP9JIVZFMEJKZRIYPLQNPSPQGZWZJZQXUVTJGRMCCJLNOLFZUCSEPNNNSYKLHJZH9YXTTTEPMDBWGXYWAMAMIDXYYSUBJKFAIH9XXBGBXMSBPJZGIDSELVW9PCTDYNKRCCZQIUIRIBNVWY9EFTZPJFLOF9GRJJQEPNOXHJHZE9KJXFX9TZZHNIVAQUSHAWTDQVGNMRMNRCKRZWCKWBBWKERTTBYKINHRYVTLVHSEDJTXVQUPBYJEQ9FFEEZOPG9HJCLPLOI9RKDDTCS9QWOZMYQJBKHRLHLCMUJODPLZFVFBINPLBLDI9EHNECSMTRWIIPVNRAWARRJSXMXCDSIENRC9MFIY9CYVLUOIWCONKRBVDRENXLXQKOGGLXWPSMQJUKUDRHBWVDQEWWSJKREESCIBIQNIWWPPWNLCBD9WYXOXCAHWLCIHTFSSNMAFPUUKZQEKWZKOYVIYSCYTOKNOSEPWPTVQBUUDUVDECYJWJQRYOPIKDLTHEAAJYQWFNMCGXRHBJTIPCPVGBVYOQTAWPHQBZEEYVNBNMHVRJDFBT9OFYRPUEIHBQIYB9TUZUMLLZAYVZKEBTQGKJPXPACTOKIG9DMUABKEFROB9FRM99JSPXZQDXTTGPPKUYMLLA9LEUFZYMWHDXTVOAUTJLC9SMEBTJMZPWNKGZTZZOYLOC9JGOQUOYYOSUSS9GNYNLROXMPFYIXPA9UOKATDFVJIGDGLMNGBCORUQMTFAQI9PDUUDRPBCRUJW9ZDHXDVGIIZLAKZQBQXZJZFZZDKKMTBMPYFEKJB9RHRZYJJMQTFLIYRHGUWEJWDD9K9INENNZPET9AJPCBPIBOZPHQTVDSCUGHFWZIDAOHXDCOUTANGUNBUHWGHXODGZCMANRSNUKFXXJLUGOZVZMFZTVSUBCGVMJAEQJFKC9HYMVNOULDFUCCXYBAGGXXDVE9ZETYAGJFXNE9DKVKDLGLYXHTFJDWKJZXUNUUVHKYRHANXJVFWVNFYWLEPMFFMMVIYRDUWSKOHDH9VFLMAKVPOVBH9GOS9TOUXDTMZPMTSCLPRUEPSNWAMVIONKWMUJYQYDZKSNCURUCARCGQUPTTVDBHQFPXMDYODFFAFTQVCJGXPZUZEZVCVVONHH9ZHLVYKUORZBGVBODHWMDMZCCQYZKQCZHHMQNPEVKTFAXFGNKCKJXQWSYKIFPVQFCPBTSCNQVHDTXBWWBGQZ9PAQCQFNSKQCAHIHOGYNVBENKJNWCBRFAU9H9ZDORYB9HDVIZOCUBP9PLCMXPEIOIOFPYWWLYWHVUJVMQCOGIMU99X9QRNURAAMROSXVYRJBK9LQCGREWFNLSPOXRGAINPAMOMZJMEAELKHJRQFLKYTEDEFGK9CNQUXPXHO9LUMZITY9MSESJJN9ZSZLNMIKLFABBKFMLGNRT9YLHUHBYMPPFXMWDPTM9T9GSBOYXSAGCRTPB9WVBOBA9QGTRSSJJUAKPZAOXNGSENLZEWOLRRFYVEGWOQJBGMXQRMDOQMLVIJKFUW9KCQHNZ9G9OBMCJSQIFPXDNQTOLFBHDHDQVBAZPBDW9SKV9TUGHW9JLPBCGLOWCFFYUCCDJARXMMZVXPIJKWTNKTXXRPFGCJUQVOASZYHDPAXFWTEQDCCZRQZCNHUXBEMLAENNPZHTID9PUCM9AQMJSJBXVH9TWUEUVRWZRKHAMPBKYYMRPXDNUWZHBCO9NQJ99MZAIBTXOFU9RDCKKIDOEACSPMIYPUFXXGBYCIVV9AHTLPPNGWJHOQBPNFKYKGCTFFEQLRPYEPMIOXLBYTKZ9YZPWXNBZVUBDAWHBDPIFCTGICEHQNTMT9AAUTI9KXAVKEZEWGFZSPVXHOVKNDXKINGSMSWGMUXHGTOAKHASIAIMEDPTPFYVE9BBSIB9OL9YBCEDHEVPCPJHTUCXFCFASRFZIDKZRSQJVEHSTKHVQXFYJFCOJDPDSQFAPEWVURE9FBSORQEXYBANRQGAWLNVPBXVEBHNULWKJJKPCXCP9QXNWVATDNRBHVWXRIQCNQMDJHMTIIHSHEYXJQVWTDASLSSISNTYMTGJUVHRPVXOZFOMYEIPK9DSLZNGEPPZDCCFGJVBJEHVSOPZANIJYYFZMSAAHNBEXJ9ONTQWMHAFKYTGUNLR9GPHWODRSIDYSJGCEOFKETUKMOBFWBXYXUVD9OAQPDDGAGXICQAVUGXGKPPZYZFNGLIYNEKTUCCWXZQLWZXDKIMQCBMCZIPN9JW9AXFNKMJMEXEJPRDJXVGLJSYUZXUPWK9E9UYBXIZXCGBRCLLWGI9RHVVUTSLYMIREQEPSMIKSG9FTOJWVECSXYERNKMSV9JZXKSTRFVYRENPUOALHGYGIRNMYBEHCZLVMPDEWEFACCJUHRJFPIX9GJZWNZLOLRIL9QJUVEENRRQEBF9OWMXEBU9APHLCTYOKBWFHIWARHPWSZWRWDPGFOGHEBHXHGIODOAG9FDMXCUNVPBPETXQSWHKLEKRHIPDZ9OYENTVRQTMNKGGLVDDIPMLFPFAKQGXQJYHRUXQNWH9STRJE9DEEPMRVBUWAZWWJUNUGBKX9ULPLYAOLKTPNLIAVDWWHK9NPFFL9QCZMXGVSWJWWC9JIJRZWJSDXSJEUYESNLINGBFBTEYMURQP9RRBD9XSNILEFSDXK9ZPRPLYJHYCWAKVOSVEOUFHBSVQOWBEKNVWKMICTUXNPROPPWGYRAPGLHFCMVWCLWEVKCASBGEGYOMJJLMDXDZPNADTSFPOFKRQKQSEULQTTJARXHKTDMNZEIVSZPIKFGTOMDFQEQEBOVGKGNC9ZMVF9AEAHEXZ9CXUAWTSGNPPUJQRREXAFJCLISFHQJUWFDNETQUCMXTEWNJUSAKRNXHA9RFYUDFYSNOFTLLYJH9YTOPWPITUBTFFGWAFXQ9CYORFC9XSUQRWEJXPWWF9IGDIYGTPLVOCFLLCHOZADUBFXQSHMXCURSCVHIJSVBBDYCYCLEEFRLIKMYHZJABDKFMWXOAVLYHKTYTWEXFUPKCPDCMTZYQRVFLGJEYFUXRDYNAJE9ZPA9XPDZCTOWZBANDDTSLI9OWYOYSGZGXWHNBQDMDGPZCMBERFPYQSBHQFFXQCK9YPBPBIOATPYJZPLJTDVYFKZFJCGSNLXJKSOYTHLJIAGLPBNLQVPBPTDSDVFNXXQRQQLNCBPAHOKWKRZFOCA9MAARTPFNYNOESMDTML99HHOIODAHDOYCULH9YNFUVWCLYECPHGVBXYVFMLYWXJU9ZTQXWBEPDWAOTMPADNUESWPQRXLJVLAKKMBRYQYLSLLBPFMZJPTKABQHMYBQAGQIYHIM9XSOEAFAYBHJLCVZIDFMNIQYXTFQCKXWWDKKKFKJWNT9DTTWLPNSOXBRVPPJMQUP9NEYJRNUWUODWZWTYHVTPSKLBPVRCERSMHFVVWJEUSHNXSYXFIBKHYRBSPAJPJ9V9UATWMVRXSCP9UVNM9ANXIXEKSXMXOXPOBHFLKIMHCEVJGAFWYFSMVNLYUSVBUHNGQNZMXIXBPUPDWAHDSIDNTTMHGEG9JFVDXGQVZMOWYRXUJWRIGTRAEVZGQDAXGILD9IQQUWAM9LHNHHRYXIYOZBDNEVORRDDOKICQCDMTDJUPIWZLEYCOOFSYOJLVKXLSBOTGAHXMLQYQEBEP9PZ9KKUOYIGECFTXXNBJIOJXMHCPJ9HOTLW9PSOHFAL9UTNUXVKF9IWMNJ9FITOC9FIYWQFSXPWAKYMIUHBK99DKLCTZUANNGVEEWEVVKMNQPQVVLG9ICNTACUTUPZYMYZKZTVEEVUGFWJGGWITRLJA9NHFYDVHGQLOBOUJHHCAHFRCFZIEXNZRLZFBVQUXOIKYKQR9JAQAZLAEYTBSREGMVEILTOWFXPHMNGGCTGLECZB"
	keyTrits := trinary.MustTrytesToTrits(key)
	digests, err := signing.Digests(keyTrits)
	if err != nil {
		// handle error
		return
	}
	fmt.Println(trinary.MustTritsToTrytes(digests))
	// output: MUVADERKIZGMEYJVHGVWBKMQMMXOPWYVOXYPNAGDNKBLHWIBUALWLWSSNDXLYAIIWX9NQRRAOQIVIHWLAIRTWWSF9TGEIKFGMCDWNIXPIYKRTSBHJIONSTSSVUCBYHS9SOZB9PSAOSJUIYQYTUV9NXLZCZWHUALYWW
}

```