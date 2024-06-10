# JavaOOP-Notes

1. Instance control classes / Utility classes / Static Factory classes

public class Contact{

   private int phonenumber;
   private String firstname;
   private String lastname;

   public Contact(){
   
   }

   public Contact(int phonenumber, String firstname, String lastname) {
    this.phonenumber = phonenumber;
    this.firstname = firstname;
    this.lastname = lastname;
   }
   
   

public int getPhonenumber() {
        return phonenumber;
    }

    public void setPhonenumber(int phonenumber) {
        this.phonenumber = phonenumber;
    }

    public String getFirstname() {
        return firstname;
    }

    public void setFirstname(String firstname) {
        this.firstname = firstname;
    }

    public String getLastname() {
        return lastname;
    }

    public void setLastname(String lastname) {
        this.lastname = lastname;
    }


    public String contactToString() {
        return "(" + firstname + ", " + lastname + ", " + phonenumber + ")";
    }

}
