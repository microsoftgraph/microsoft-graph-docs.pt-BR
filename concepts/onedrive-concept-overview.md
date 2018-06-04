# <a name="onedrive-file-storage-api-overview"></a><span data-ttu-id="e767e-101">Visão geral da API de armazenamento de arquivos do OneDrive</span><span class="sxs-lookup"><span data-stu-id="e767e-101">OneDrive file storage API overview</span></span>

<span data-ttu-id="e767e-102">O OneDrive é a central de arquivos no Office 365.</span><span class="sxs-lookup"><span data-stu-id="e767e-102">OneDrive is the files hub in Office 365.</span></span>
<span data-ttu-id="e767e-103">As pessoas trabalham com arquivos em vários contextos, como o Microsoft Teams, grupos, SharePoint e muito mais.</span><span class="sxs-lookup"><span data-stu-id="e767e-103">People work with files in a variety of contexts, like Microsoft Teams, groups, SharePoint, and more.</span></span>
<span data-ttu-id="e767e-104">Com o OneDrive, os usuários podem acessar esses arquivos independentemente de onde eles estejam armazenados; com o Microsoft Graph, você pode usar uma única API para trabalhar com eles.</span><span class="sxs-lookup"><span data-stu-id="e767e-104">With OneDrive, users can access these files no matter where they are stored, and with Microsoft Graph, you can use a single API to work with them.</span></span>

<span data-ttu-id="e767e-105">Os arquivos no Office 365 são armazenados em [unidades][Drive API].</span><span class="sxs-lookup"><span data-stu-id="e767e-105">Files in Office 365 are stored in [drives][Drive API].</span></span>
<span data-ttu-id="e767e-106">Os usuários podem armazenar arquivos em uma unidade pessoal, o OneDrive pessoal, ou em uma unidade compartilhada com a tecnologia de uma biblioteca de documentos do [SharePoint][].</span><span class="sxs-lookup"><span data-stu-id="e767e-106">Users can store files in a personal drive - their OneDrive - or in a shared drive powered by a [SharePoint][] document library.</span></span>
<span data-ttu-id="e767e-107">A flexibilidade do OneDrive permite que os usuários colaborem como acharem melhor para eles.</span><span class="sxs-lookup"><span data-stu-id="e767e-107">OneDrive's flexibility lets users collaborate however it works best for them.</span></span>
<span data-ttu-id="e767e-108">Os usuários podem compartilhar links para arquivos, copiar ou mover arquivos para unidades da equipe ou até mesmo anexar arquivos do OneDrive às mensagens de email no Outlook.</span><span class="sxs-lookup"><span data-stu-id="e767e-108">Users can share links to files, copy or move files to team drives, or even attach OneDrive files to mail messages in Outlook.</span></span>

## <a name="why-integrate-with-onedrive-file-storage-in-the-cloud"></a><span data-ttu-id="e767e-109">Por que se integrar ao armazenamento de arquivos do OneDrive na nuvem?</span><span class="sxs-lookup"><span data-stu-id="e767e-109">Why integrate with OneDrive file storage in the cloud?</span></span>

### <a name="tap-into-an-ecosystem-with-billions-of-files"></a><span data-ttu-id="e767e-110">Utilize um ecossistema com bilhões de arquivos</span><span class="sxs-lookup"><span data-stu-id="e767e-110">Tap into an ecosystem with billions of files</span></span>

<span data-ttu-id="e767e-111">Os usuários do OneDrive podem acessar seus arquivos de qualquer dispositivo, online ou offline, e compartilhar arquivos com pessoas de dentro ou de fora da organização.</span><span class="sxs-lookup"><span data-stu-id="e767e-111">OneDrive users can access their files from any device, online or offline, and share files with people inside or outside their organization.</span></span>
<span data-ttu-id="e767e-112">O OneDrive permite a coautoria em tempo real em aplicativos conhecidos, como o Word, o Excel e o PowerPoint.</span><span class="sxs-lookup"><span data-stu-id="e767e-112">OneDrive enables real-time coauthoring in familiar apps like Word, Excel, and PowerPoint.</span></span>
<span data-ttu-id="e767e-113">Os arquivos ficam ainda melhores com miniaturas avançadas para centenas de formatos, transmissão de vídeo, análises, entre outros, com base na tecnologia do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="e767e-113">Files light up with rich thumbnails for hundreds of formats, video streaming, analytics, and more, powered by Microsoft Graph.</span></span>
<span data-ttu-id="e767e-114">Os dados no OneDrive são protegidos com recursos avançados de segurança, conformidade e a criptografia em que os clientes confiam.</span><span class="sxs-lookup"><span data-stu-id="e767e-114">Data in OneDrive is protected with advanced encryption, compliance, and security features that customers trust.</span></span>

<span data-ttu-id="e767e-115">Com mais de 500 milhões de dispositivos executando o aplicativo do OneDrive e mais de 85% das empresas da Fortune 500 usando o OneDrive for Business, ao integrar o aplicativo ao OneDrive você pode se conectar com milhões de clientes, alunos e usuários corporativos e interagir com os clientes de onde eles já trabalham todo dia.</span><span class="sxs-lookup"><span data-stu-id="e767e-115">With over 500 million devices running the OneDrive app and over 85% of the Fortune 500 using OneDrive for Business, by integrating your app with OneDrive, you can connect with millions of consumers, students, and business users and engage with customers where they already do their work every day.</span></span>

### <a name="store-your-apps-files-in-a-powerful-cloud"></a><span data-ttu-id="e767e-116">Armazenar os arquivos do seu aplicativo em uma nuvem avançada</span><span class="sxs-lookup"><span data-stu-id="e767e-116">Store your app's files in a powerful cloud</span></span>

<span data-ttu-id="e767e-117">Quando você armazena seus arquivos no OneDrive, seu aplicativo pode utilizar os recursos da nuvem da Microsoft e seus usuários podem acessar os arquivos de qualquer lugar.</span><span class="sxs-lookup"><span data-stu-id="e767e-117">When you store your files in OneDrive, your app can take advantage of the features of the Microsoft cloud and your users can access their files anywhere.</span></span>
<span data-ttu-id="e767e-118">Use a SDK do [seletor de arquivos][] para rapidamente abrir, baixar, salvar ou compartilhar os arquivos armazenados no OneDrive do próprio aplicativo, usando a mesma experiência que os usuários do OneDrive já conhecem.</span><span class="sxs-lookup"><span data-stu-id="e767e-118">Use the [file picker][] SDK to quickly open, download, save, or share files stored in OneDrive from within your own app, using the same experience OneDrive users are familiar with.</span></span>
<span data-ttu-id="e767e-119">Obtenha informações sobre os arquivos selecionados diretamente do SDK do seletor ou use diretamente as APIs do Microsoft Graph para interagir de forma mais profunda com os arquivos.</span><span class="sxs-lookup"><span data-stu-id="e767e-119">Get information about selected files directly from the picker SDK, or use Microsoft Graph APIs directly to interact more deeply with files.</span></span>
<span data-ttu-id="e767e-120">Use [pastas especiais][] para armazenar arquivos em locais conhecidos no OneDrive, como `Documents` e `Camera Roll`, ou crie uma pasta pessoal para o seu aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e767e-120">Use [special folders][] to store files in well-known locations on OneDrive, like `Documents` and `Camera Roll`, or give your app its own personal folder.</span></span>

### <a name="bring-your-app-straight-to-users-within-onedrive"></a><span data-ttu-id="e767e-121">Disponibilizar o seu aplicativo diretamente para os usuários no OneDrive</span><span class="sxs-lookup"><span data-stu-id="e767e-121">Bring your app straight to users within OneDrive</span></span>

<span data-ttu-id="e767e-122">Os clientes do OneDrive podem usar ou iniciar o seu aplicativo diretamente do OneDrive para abrir, editar ou visualizar arquivos.</span><span class="sxs-lookup"><span data-stu-id="e767e-122">OneDrive customers can use or launch your app directly from within OneDrive to open, edit, or preview files.</span></span>
<span data-ttu-id="e767e-123">Use as extensões do [manipulador de arquivos][] do OneDrive para fornecer ícones e visualizações para as suas próprias extensões de arquivo personalizado, adicionar o seu aplicativo ao botão **Novo** ou até mesmo adicionar as suas próprias ações personalizadas à barra de menus para iniciar o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="e767e-123">Use OneDrive's [file handler][] extensions to provide icons and previews for your own custom file extensions, add your app to the **New** button or even add your own custom actions to the menu bar to launch your app.</span></span>

### <a name="work-with-content-in-formats-your-app-understands"></a><span data-ttu-id="e767e-124">Trabalhar com conteúdo em formatos que o seu aplicativo entende</span><span class="sxs-lookup"><span data-stu-id="e767e-124">Work with content in formats your app understands</span></span>

<span data-ttu-id="e767e-125">O aplicativo pode obter o conteúdo do arquivo no formato que for mais conveniente para você.</span><span class="sxs-lookup"><span data-stu-id="e767e-125">Your app can get file content in the format that is most convenient for you.</span></span>
<span data-ttu-id="e767e-126">O aplicativo pode exibir [miniaturas][] de tamanho personalizado para centenas de formatos diferentes de arquivo.</span><span class="sxs-lookup"><span data-stu-id="e767e-126">Your app can display custom-sized [thumbnails][] for hundreds of different file formats.</span></span>
<span data-ttu-id="e767e-127">Você pode baixar arquivos em vários [formatos][] alternativos, como PDF.</span><span class="sxs-lookup"><span data-stu-id="e767e-127">You can download files in a variety of alternative [formats][], like PDF.</span></span>
<span data-ttu-id="e767e-128">Você pode inclusive inserir visualizadores de arquivo do OneDrive no seu aplicativo usando a API de [visualização][] (beta).</span><span class="sxs-lookup"><span data-stu-id="e767e-128">You can even embed the OneDrive file previewers within your app by using the [preview][] API (beta).</span></span>

### <a name="work-with-file-content-and-metadata-without-downloading-the-binary"></a><span data-ttu-id="e767e-129">Trabalhar com conteúdo e metadados de arquivo sem baixar o binário</span><span class="sxs-lookup"><span data-stu-id="e767e-129">Work with file content and metadata without downloading the binary</span></span>

<span data-ttu-id="e767e-130">Com o Microsoft Graph, é possível acessar conteúdo avançado por meio de APIs REST sem precisar baixar o binário.</span><span class="sxs-lookup"><span data-stu-id="e767e-130">With Microsoft Graph, you can access rich content through REST APIs without having to download the binary.</span></span>
<span data-ttu-id="e767e-131">Explore os metadados extraídos dos arquivos de [foto][], [áudio][] e [vídeo][].</span><span class="sxs-lookup"><span data-stu-id="e767e-131">Explore extracted metadata from [photo][], [audio][], and [video][] files.</span></span>
<span data-ttu-id="e767e-132">Use a [API do Excel][] para trabalhar diretamente com os dados brutos armazenados em uma pasta de trabalho do Excel.</span><span class="sxs-lookup"><span data-stu-id="e767e-132">Use the [Excel API][] to work directly with the raw data stored in an Excel workbook.</span></span>
<span data-ttu-id="e767e-133">Use a [API de anotações][] para acessar o conteúdo dos blocos de anotações do OneNote.</span><span class="sxs-lookup"><span data-stu-id="e767e-133">Use the [Notes API][] to access the contents of OneNote notebooks.</span></span>

### <a name="react-to-file-changes"></a><span data-ttu-id="e767e-134">Reagir a alterações de arquivo</span><span class="sxs-lookup"><span data-stu-id="e767e-134">React to file changes</span></span>

<span data-ttu-id="e767e-135">Com o [webhooks][], seu aplicativo pode ser notificado sobre a alteração de arquivos, o que possibilita que você reaja rapidamente.</span><span class="sxs-lookup"><span data-stu-id="e767e-135">With [webhooks][], your app can get notified when files change so you can quickly react.</span></span>
<span data-ttu-id="e767e-136">Use a [API delta][] para ver o que foi alterado desde a última vez que o aplicativo foi sincronizado com a nuvem.</span><span class="sxs-lookup"><span data-stu-id="e767e-136">Use the [delta API][] to see what changed since the last time your app synchronized with the cloud.</span></span>

## <a name="next-steps"></a><span data-ttu-id="e767e-137">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="e767e-137">Next steps</span></span>

<span data-ttu-id="e767e-138">Saiba mais sobre [como usar a API do OneDrive][Drive API] no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="e767e-138">Find out more about [using the OneDrive API][Drive API] in Microsoft Graph v1.0.</span></span>

[SharePoint]: sharepoint-concept-overview.md
[seletor de arquivos]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[File picker]: https://dev.onedrive.com/sdk/js-v72/js-picker-overview.htm
[manipulador de arquivos]: https://docs.microsoft.com/onedrive/developer/file-handlers
[file handler]: https://docs.microsoft.com/onedrive/developer/file-handlers
<span data-ttu-id="e767e-142">
  [pastas especiais]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span><span class="sxs-lookup"><span data-stu-id="e767e-142">[Special folders]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/drive_get_specialfolder</span></span>
<span data-ttu-id="e767e-143">
  [API de anotações]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span><span class="sxs-lookup"><span data-stu-id="e767e-143">[Notes API]: https://developer.microsoft.com/en-us/graph/docs/concepts/integrate_with_onenote</span></span>
<span data-ttu-id="e767e-144">
  [API do Excel]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span><span class="sxs-lookup"><span data-stu-id="e767e-144">[Excel API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/excel</span></span>
[REST API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
<span data-ttu-id="e767e-145">
  [API delta]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span><span class="sxs-lookup"><span data-stu-id="e767e-145">[delta API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_delta</span></span>
<span data-ttu-id="e767e-146">
  [vídeo]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span><span class="sxs-lookup"><span data-stu-id="e767e-146">[video]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/video</span></span>
<span data-ttu-id="e767e-147">
  [foto]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span><span class="sxs-lookup"><span data-stu-id="e767e-147">[photo]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/photo</span></span>
<span data-ttu-id="e767e-148">
  [áudio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span><span class="sxs-lookup"><span data-stu-id="e767e-148">[audio]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/audio</span></span>
<span data-ttu-id="e767e-149">
  [formatos]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span><span class="sxs-lookup"><span data-stu-id="e767e-149">[Formats]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_get_content_format</span></span>
<span data-ttu-id="e767e-150">
  [miniaturas]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span><span class="sxs-lookup"><span data-stu-id="e767e-150">[thumbnails]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/api/driveitem_list_thumbnails</span></span>
<span data-ttu-id="e767e-151">
  [visualização]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span><span class="sxs-lookup"><span data-stu-id="e767e-151">[Preview]: https://developer.microsoft.com/en-us/graph/docs/api-reference/beta/api/driveitem_preview</span></span>
<span data-ttu-id="e767e-152">
  [webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span><span class="sxs-lookup"><span data-stu-id="e767e-152">[Webhooks]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/webhooks</span></span>
[Drive API]: https://developer.microsoft.com/en-us/graph/docs/api-reference/v1.0/resources/onedrive
