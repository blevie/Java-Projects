/**
 * Predefined rotors for Enigma encryption.
 * Rotor ciphers are based off of those found in the M3 Enigma Machine.
 * 
 * @author Seth Pollen pollen@cs.wisc.edu
 */
public class RotorConstants {
	
	
	/** The number of letters printed on each rotor. */
	public static final int ROTOR_LENGTH = 26;
	
	/**
	 * The cipher strings for each rotor. They store the letter-order
	 * for each rotor. The rotor at index 0 is the identity rotor.
	 * The identity rotor will be useful for debugging. 
	 * 
	 * The remaining cipher strings correspond to:
	 * Rotor I, Rotor II, etc.
	 * 
	 * <p>Real rotor data was found at:
	 * http://en.wikipedia.org/wiki/Enigma_rotor_details#Rotor_wiring_tables
	 */
	public static final String[] ROTORS = {

		// Identity Rotor (index 0 - and useful for testing):
		"ABCDEFGHIJKLMNOPQRSTUVWXYZ",
		
		// Standard Rotors I through VIII:
		"EKMFLGDQVZNTOWYHXUSPAIBRCJ",
		"AJDKSIRUXBLHWTMCQGZNPYFVOE",
		"BDFHJLCPRTXVZNYEIWGAKMUSQO",
		"ESOVPZJAYQUIRHXLNFTGKDCMWB",
		"VZBRGITYUPSDNHLXAWMJQOFECK",
		"JPGVOUMFYQBENHZRDKASXLICTW",
		"NZJHGRCXMYSWBOUFAIVLPEKQDT",
		"FKQHTLXOCBJSPDZRAMEWNIUYGV",
	};
	
	/**
	 * This is a String constant which represents the letters to be 
     * printed on the special Reflector rotor. The reflector rotor is placed 
     * at the end of the stack of other rotors. 
     * 
     * It cipher has the special property that every pair of characters 
     * map to each other. 
	 */
	public static final String REFLECTOR = "QYHOGNECVPUZTFDJAXWMKISRBL";
	// To better see the reflection:        ABCDEFGHIJKLMNOPQRSTUVWXYZ
	
	/**
	 * The locations of each rotors' step notches. Each rotor has one or 
	 * two step notches next to particular encoded letters. 
	 * 
	 * When a rotor is turned into the position of its step notch,
	 * it also causes the next rotor to advance by one position.
	 * 
	 * <p> Each rotor may have one or more notches. 
	 * This array has a 1-to-1 correspondence with the ROTORS array. 
	 * That is, the rotor in index 0 of ROTORS will correspond to the values 
	 * stored at NOTCHES index 0.
	 * 
	 * <p>Each rotor may have a different number of notches, 
	 * so this 2D array does not have the same number of elements in 
	 * each sub-array</p>
	 */
	public static final int[][] NOTCHES = {
		// Identity rotor:
		{ 0 }, // A
		
		// Standard rotors:
		{ 17 }, // Rotor I:   notch at R
		{ 5 },  // Rotor II:  notch at F
		{ 22 }, // Rotor III: notch at W
		{ 10 }, // Rotor IV:  notch at K
		{ 0 },  // Rotor V:   notch at A
		
		// The last three rotors have two step notches each.
		{ 0, 13 }, // Rotor VI:   notch at A and N
		{ 0, 13 }, // Rotor VII:  notch at A and N
		{ 0, 13 }, // Rotor VIII: notch at A and N
	};
	
}
