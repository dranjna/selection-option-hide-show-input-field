# selection-option-hide-show-input-field
## Add in html
`<div class="form-group  w-50" id="add-product-input-field" style="display: none;">
                                        <label for="location2" style="font-weight:bold;">Parent Category</label>
                                        <select class="custom-select form-control" id="select_item" name="location">
                                            <option value="">Select parent category</option>
                                            <option value="1">Home and Kitchen </option>
                                            <option value="2">Computers </option>
                                            <option value="3">Clothing </option>
                                            <option value="4">Sports </option>
                                            <option value="5">Others </option>
                                        </select>
                                    </div>
                                    </div>
                                    <div class="row justify-content-center">
                                    <div class="form-group w-50" id="home-kitchen-input-field" style="display: none;">
                                        <label for="location2" style="font-weight:bold;">Level 1 Category</label>
                                        <select class="custom-select form-control" id="location2" name="location">
                                            <option value=""> Artwork </option>
                                            <option value="Amsterdam"> Home Decor </option>
                                            <option value="Berlin"> Bedding </option>
                                            <option value="Frankfurt"> Heating, Cooling & Air Quality </option>
                                            <option value="sports"> Iron & Steamers </option>
                                            <option value="others"> Furniture </option>
                                            <option value="others"> Bath Rugs </option>
                                            <option value="others"> Bath Towels </option>
                                            <option value="others"> Kitchen & Dinning </option>
                                        </select>
                                    </div>`
                                    
 ##add in jquery
 `<script>
        document.getElementById('select_item').addEventListener('change', function () {
            var style = this.value == 1 ? 'block' : 'none';
            document.getElementById('home-kitchen-input-field').style.display = style;
        });
    </script>`
