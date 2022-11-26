<template>
  <div class="contact-about">
            <h2>Contact Us</h2>
            <div class="content">
                <div class="form-dev">
                    <form action="">
                        <div class="">
                            <div class="form-group">
                                <label for="name" class="col-md-12 control-label pb-2 pt-2">Name:</label>
                                <input id="name" type="text" class="form-control col-md-12" name="name" value="" required>
                            </div>
                            <div class="form-group">
                                 <label for="email" class="col-md-12 control-label pb-2 pt-2">E-mail:</label>
                                <input id="email" type="email" class="form-control col-md-12" name="email" value="" required>
                            </div>
                            <div class="form-group">
                                 <label for="phone" class="col-md-12 control-label pb-2 pt-2">Phone:</label>
                                <input id="phone" type="text" class="form-control col-md-12" name="phone" value="" required>
                            </div>
                        </div>
                        <div class="">
                            <div class="form-group">
                                 <label for="message" class="col-md-12 control-label pb-2 pt-2">Your Message:</label>
                                <textarea name="message" id="message" cols="50" rows="10"></textarea>
                            </div>
                        </div>
                    </form>
                </div>
                <div class="contact-dev">
                    <h2>Dubai</h2>
                    <div class="contact">
                        <div class="image">
                            <img src="../../public/assets/images/icon/Asset 26ldpi.png" alt="">
                        </div>
                        <div class="content">
                            <p>Mr. Ahmad Abdullah</p>
                            <p>+971 4 8871193/94</p>
                            <p>+971 4 8871193/94</p>
                            <p>+971 4 8871193/94</p>
                            <p>toheco@toheco.com</p>
                        </div>
                    </div>
                    <div class="btn-contact">
                        <button>Send message</button>
                    </div>
                </div>
            </div>
        </div>
</template>

<script>
export default {
  name: "ContactAbout"
};
</script>

