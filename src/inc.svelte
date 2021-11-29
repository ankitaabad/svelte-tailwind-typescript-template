<!-- card component -->

<!-- form component -->
<script>
  let selected = true;
  const toggle_selected = ()=>{
    selected ^=true;
  }
</script>
<div class="flex flex-col border-2 md:w-1/4 shadow-md px-4 pt-3 pb-5">
  <label for="card_number" class="font-semibold">Card Number</label>
  <input
    type="text"
    name="card_number"
    id="card_number"
    class=" border-gray-400 focus:shadow-lg h-7 rounded-md pl-2"
  />
  <label for="card_name" class="mt-2  font-semibold">Card Name</label>
  <input
    type="text"
    name="card_name"
    id="card_name"
    class=" border-gray-400 focus:shadow-lg h-7 rounded-md pl-2"
  />
  <div class="mt-2 flex flex-row gap-2" class:bg-blue-50={selected}>
    <div class="flex-grow">
      <label for="expiration_date" class="font-semibold">Expiration Date</label>
      <div class="flex flex-row gap-4 h-7">
        <select name="" class="w-1/2 rounded-md" id="">
          <option>1</option>;
        </select>
        <select class="w-1/2 rounded-md">
          <option>2021</option>

          <option>2020</option>
        </select>
      </div>
    </div>
    <div class="ml-4">
      <label for="cvv" class="font-semibold">cvv</label>
      <input type="text" class="w-16 pl-2" />
    </div>
  </div>
  <button
    class="bg-blue-700 text-white h-9 mt-2 font-semibold shadow-md rounded-md hover:bg-blue-600 font-sans" on:click={toggle_selected}
    >Submit</button
  >
</div>
