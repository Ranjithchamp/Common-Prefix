# Common-Prefix
import java.util.Scanner;

public class CommonPrefix {

	public static void main(String[] args) {
		Scanner qq = new Scanner(System.in);
		String[] inp = { "Hai", "Had", "Hate" };
		String sub = inp[0];
		for (int i = 0; i < inp.length; i++) {
			while (!sub.equals("")) {
				if (inp[i].startsWith(sub)) {

					break;
				} else {
					sub = sub.substring(0, sub.length() - 1);
				}

			}

		}
		if (sub.equals("")) {
			System.out.println("Their is no common Prefix");
		} else {
			System.out.println("The common Prefix is : " + sub);
		}
	}

}
