# Baba-xml
xml files from various sources plus word docs from transcribing the underlying tapes
Brad Gunn and others (currently Ed Flanagan, Jerry Carlin, Ursula Reinhart, and Jack Mormon have all
contributed audio tapes of various mandali speaking at mandali hall and other locations. Speakers
include Adi, Meherjee, Eruch, Mani, Arnavaz, Goher, Kohiyar Satarawala and various others. Westerners
and other visitors appear from time to time on the tapes, particularly in Mandali Hall where Eruch
liked to hear others tell their stories. 

It became difficult to maintain version control over the transcriptions, particularly as the xml changed a bit
So this repo was born for that purpose. In addition, Nosherwan wanted Microsoft Word documents for his own 
collection, and in making them the xnl <content> tag's contents tended to become obsolete, so those are included 
here as well.

The tag structure of the xml files, at least from 2000 to 2019, has remained as in this example:
<?xml version="1.0" encoding="utf-8"?> -- every xml file starts with this
<tape_side number="(e.g.,the phusical label on the tape" brad_number="T#163">
<segment> -- every tape has the potential for multiple segments, separated according to the time when they were recorded
<speakers>
  <speaker>Eruch</speaker>
  <speaker>Mani</speaker> -- and of course more as required
  </speakers>
<dates>
  <date><year>1979</year><month>3</month><day>4</day></date>
  </dates>
<continuation_of>kg072b</continuation_of>
  <persons_present>
<person_present>Christina</person_present>
<person_present>LA center president</person_present>
<person_present>Craig</person_present>
  </persons_present>
<keys>
  <key>What this is about in a nutshell</key>
  </keys>
<content>
  </content>
  </segment>
/* and then optionally the same structure repeated for another segment. One tape has three or four segments, but most have
only one. */
</tape_side>
