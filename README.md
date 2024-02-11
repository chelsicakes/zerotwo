
<!DOCTYPE html>

<head>
  <title>Mapua GWA Calculator</title>
  <link
    href="https://unpkg.com/tailwindcss@1.4.6/dist/tailwind.css"
    rel="stylesheet"
  />
  <link
    rel="shortcut icon"
    href="https://img.icons8.com/color/48/000000/html-5.png"
  />

  <script type="text/javascript" src="https://livejs.com/live.js"></script>
</head>

<body class="min-h-screen">
  <div
    class="item-stretch w-screen px-5 lg:container lg:w-5/6 xl:w-2/3 mx-auto p-2 lg:p-5 lg:shadow-2xl"
  >
    <img
      src="https://img.icons8.com/color/240/000000/html-5.png"
      class="mx-auto h-40 lg:h-24"
    />
    <h1 class="text-center text-6xl lg:text-4xl font-bold pb-10">
      Mapua GWA Calculator
    </h1>
    <form id="tblForm">
      <table class="table-fixed w-full">
        <thead>
          <tr>
            <th class="w-full px-5 py-2 text-3xl lg:text-xl">SUBJECT</th>
            <th class="w-full px-5 py-2 text-3xl lg:text-xl">GRADE</th>
            <th class="w-full px-5 py-2 text-3xl lg:text-xl">UNITS</th>
          </tr>
        </thead>
        <tbody id="tbody">
          <!-- <tr>
            <td class="border-2 border-gray-600 shadow-md">
              <input
                class="w-full py-5 lg:py-1 text-center text-4xl lg:text-base focus:outline-none"
              />
            </td>
            <td class="border-2 border-gray-600 shadow-md">
              <input
                class="w-full py-5 lg:py-1 text-center text-4xl lg:text-base focus:outline-none"
              />
            </td>
            <td class="border-2 border-gray-600 shadow-md">
              <input
                class="w-full py-5 lg:py-1 text-center text-4xl lg:text-base focus:outline-none"
              />
            </td>
          </tr> -->
        </tbody>
      </table>
    </form>
    <div class="container w-full mx-auto pt-5 text-center">
      <button
        id="clearAll"
        onClick="clearAll()"
        class="focus:outline-none text-4xl lg:text-lg rounded-lg bg-red-500 hover:bg-red-400 text-white font-bold py-2 px-4 border-b-4 border-red-700 hover:border-red-500 rounded"
      >
        Clear all
      </button>
      <button
        id="removeRow"
        onClick="removeRow()"
        class="focus:outline-none text-4xl lg:text-lg rounded-lg bg-red-500 hover:bg-red-400 text-white font-bold py-2 px-4 border-b-4 border-red-700 hover:border-red-500 rounded"
      >
        Remove row
      </button>
      <button
        id="addSub"
        onClick="addSub()"
        class="focus:outline-none text-4xl lg:text-lg rounded-lg bg-blue-500 hover:bg-blue-400 text-white font-bold py-2 px-4 border-b-4 border-blue-700 hover:border-blue-500 rounded"
      >
        Add Subject
      </button>
      <br /><br />
      <button
        id="compute"
        onClick="compute()"
        class="focus:outline-none text-5xl lg:text-lg rounded-lg bg-blue-500 hover:bg-blue-400 text-white font-bold py-2 px-4 border-b-4 border-blue-700 hover:border-blue-500 rounded"
      >
        Compute
      </button>
    </div>
    <div class="container w-full mx-auto pt-5 text-center">
      <p id="GWA" class="text-5xl lg:text-lg"></p>
    </div>

    <footer class="pt-10 text-2xl lg:text-base">
      Lagyan mo lahat ng GRADE at UNITS. Kahit di mo na lagyan yung subject.
    </footer>
  </div>

  <script src="./index.js"></script>
</body>
