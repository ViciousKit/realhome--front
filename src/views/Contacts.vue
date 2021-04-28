<template>
    <div class="container contacts">
        <div class="col-md-12 about_us_link about_us_link_contacts"><a href="">Home</a><b>-></b> About Us</div>
        <h1 class="contacts_title">Out <b>Contacts</b></h1>
        <div class="col-md-12 text-center">
            <iframe src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2242.7905889307344!2d37.69835751604762!3d55.7968740960594!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x46b535a0cc9501f3%3A0xfc1e2c28d2cc40a2!2z0JrQvtC70L7QtNC10LfQvdGL0Lkg0L_QtdGALiwg0LQuMywg0JzQvtGB0LrQstCwLCAxMDcwNzY!5e0!3m2!1sru!2sru!4v1619607296476!5m2!1sru!2sru" width="800" height="600" style="border:0;" allowfullscreen="" loading="lazy"></iframe>
        </div>
        <div class="d-flex flex-row contacts_block">
            <div class="d-flex flex-column contacts_block_info">
                <h1 class="contacts_block_title">Contact Info</h1>
                <p class="contacts_block_info_text">Etiam commodo consequat egestas. Morbi at ligula nulla. Mauris bibendum mi vitae condimentum mollis. Sed sollicitudin enim vehicula, varius sapien id, consectetur posuere sem commodo.</p>
                <h4 class="contacts_block_info_aboutCompany">Real Home INC. <br> ST STEPHEN'S HOUSE, COLSTON AVE, <br> BRISTOL, BRISTOL BS1 4ST, UK</h4>
                <div class="contacts_block_info_contacts">
                    <p>Telephone: <b>+1 800 603 6035</b></p>
                    <p>FAX: <b>+1 800 889 9898</b></p>
                    <p>E-mail: <a href="">mail@demolink.org</a></p>
                </div>
            </div>
            <div class="d-flex flex-column contacts_block_commentInput">
                <h1 class="contacts_block_title">Leave a Comment</h1>
                <div class="input-group contacts_input mb-3">
                    <input type="name" class="form-control name" id="exampleFormControlInput1" placeholder="Your name">
                    <span class="space"></span>
                    <input type="email" class="form-control email" id="exampleFormControlInput1" placeholder="Your email">
                </div>
                <div class="mb-3">
                    <textarea class="form-control" id="exampleFormControlTextarea1" placeholder="Your Comment" rows="3"></textarea>
                </div>
                <div class="col-md-3">
                    <button class="btn btn-primary btn-contacts btn_send">SEND</button>
                    <button class="btn btn-primary btn-contacts btn_clear disabled">CLEAR</button>
                </div>
            </div>
        </div>
    </div>
</template>