# <a name="getting-started-building-microsoft-graph-apps"></a><span data-ttu-id="b3a9a-101">Introdução à criação de aplicativos do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="b3a9a-101">Getting started building Microsoft Graph apps</span></span>

<span data-ttu-id="b3a9a-p101">Os artigos desta seção fornecem orientações detalhadas sobre como criar aplicativos que se conectam ao Microsoft Graph em uma variedade de linguagens e plataformas de desenvolvimento. Cada artigo começa com um exemplo de projeto inicial para a plataforma apropriada e orienta para que você consiga adicionar funcionalidades que autenticam o usuário e fazem um exemplo de solicitação para que o Microsoft Graph envie um email da sua conta. O projeto concluído é idêntico ao [Exemplo de conexão no repositório do Microsoft Graph](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) para essa plataforma.</span><span class="sxs-lookup"><span data-stu-id="b3a9a-p101">The articles in this section provide detailed guidance on how to build apps that connect to Microsoft Graph across a variety of languages and development platforms. Each article starts with a sample starter project for the appropriate platform, and walks you through adding functionality that authenticates the user and makes a sample request to have Microsoft Graph send an email from their account. The completed project is identical to the [Connect sample in the Microsoft Graph repo](https://github.com/microsoftgraph?utf8=%E2%9C%93&query=connect) for that platform.</span></span>

<span data-ttu-id="b3a9a-105">Escolha o artigo correspondente ao provedor de autenticação e à plataforma de desenvolvimento de sua escolha e comece a conexão com o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b3a9a-105">Choose the article that covers the authentication provider and development platform of your choice, and get started connecting to Microsoft Graph.</span></span>

<span data-ttu-id="b3a9a-106">Você pode seguir as etapas no artigo que aborda a plataforma de desenvolvimento que você escolheu ou, para obter rapidamente uma solução que funcione, tente a experiência de [início rápido](https://developer.microsoft.com/graph/quick-start).</span><span class="sxs-lookup"><span data-stu-id="b3a9a-106">You can follow the steps in the article that covers the development platform that you choose, or, to quickly get a working solution up and running, try out the [quick start](https://developer.microsoft.com/graph/quick-start) experience.</span></span>

<span data-ttu-id="b3a9a-p102">Para explorar os exemplos de Conexão concluídos, confira [Microsoft Graph](https://github.com/microsoftgraph) no GitHub. A tabela a seguir mostra os exemplos por provedor e plataforma de autenticação e observa se eles se conectam ao Microsoft Graph usando REST ou uma biblioteca de cliente do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="b3a9a-p102">To explore the finished Connect samples, see [Microsoft Graph](https://github.com/microsoftgraph) in GitHub. The following table lists the samples by authentication provider and platform, and notes whether they connect to Microsoft Graph using REST or a Microsoft Graph client library.</span></span>

<table>
  <tr>
    <th><span data-ttu-id="b3a9a-109">Plataforma</span><span class="sxs-lookup"><span data-stu-id="b3a9a-109">Platform</span></span></th>
    <th><span data-ttu-id="b3a9a-110">Ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="b3a9a-110">Azure AD endpoint</span></span></th> 
    <th><span data-ttu-id="b3a9a-111">Ponto de extremidade do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="b3a9a-111">Azure AD v2.0 endpoint</span></span></th>
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-112">Android</span><span class="sxs-lookup"><span data-stu-id="b3a9a-112">Android</span></span></td>
    <td><span data-ttu-id="b3a9a-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-113">
        <a href="https://github.com/microsoftgraph/android-java-connect-sample/tree/last_v1_auth">SDK sample</a>
    </span></span></td> 
        <td><span data-ttu-id="b3a9a-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">Exemplo de SDK</a> ou ¶<a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-114">
                <a href="https://github.com/microsoftgraph/android-java-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/android-java-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-115">AngularJS</span><span class="sxs-lookup"><span data-stu-id="b3a9a-115">AngularJS</span></span></td>
    <td><span data-ttu-id="b3a9a-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-116">
        <a href="https://github.com/microsoftgraph/angular-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td> 
        <td><span data-ttu-id="b3a9a-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">Exemplo de SDK</a> ou ¶<a href="https://github.com/microsoftgraph/angular-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-117">
        <a href="https://github.com/microsoftgraph/angular-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/angular-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-118">ASP.NET</span><span class="sxs-lookup"><span data-stu-id="b3a9a-118">ASP.NET</span></span></td>
    <td><span data-ttu-id="b3a9a-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-119">
        <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="b3a9a-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">Exemplo de SDK</a> ou ¶<a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-120">
        <a href="https://github.com/microsoftgraph/aspnet-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/aspnet-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-121">iOS (Obj-C)</span><span class="sxs-lookup"><span data-stu-id="b3a9a-121">iOS (Obj-C)</span></span></td>
    <td><span data-ttu-id="b3a9a-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-122">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="b3a9a-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-123">
        <a href="https://github.com/microsoftgraph/ios-objectivec-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-124">iOS (Swift)</span><span class="sxs-lookup"><span data-stu-id="b3a9a-124">iOS (Swift)</span></span></td>
    <td><span data-ttu-id="b3a9a-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-125">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="b3a9a-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-126">
        <a href="https://github.com/microsoftgraph/ios-swift-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-127">NodeJS</span><span class="sxs-lookup"><span data-stu-id="b3a9a-127">NodeJS</span></span></td>
    <td><span data-ttu-id="b3a9a-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-128">
        <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td>    
        <span data-ttu-id="b3a9a-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">Exemplo de SDK</a> ou <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-129"><a href="https://github.com/microsoftgraph/nodejs-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/nodejs-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-130">PHP</span><span class="sxs-lookup"><span data-stu-id="b3a9a-130">PHP</span></span></td>
    <td><span data-ttu-id="b3a9a-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-131">
        <a href="https://github.com/microsoftgraph/php-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="b3a9a-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">Exemplo de SDK</a> ou ¶<a href="https://github.com/microsoftgraph/php-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-132">
            <a href="https://github.com/microsoftgraph/php-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/php-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-133">Python</span><span class="sxs-lookup"><span data-stu-id="b3a9a-133">Python</span></span></td>
    <td><span data-ttu-id="b3a9a-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-134">
        <a href="https://github.com/microsoftgraph/python3-connect-rest-sample">REST sample</a>
    </span></span></td>     
    <td>
    </td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-135">Ruby</span><span class="sxs-lookup"><span data-stu-id="b3a9a-135">Ruby</span></span></td>
    <td><span data-ttu-id="b3a9a-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-136">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="b3a9a-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-137">
        <a href="https://github.com/microsoftgraph/ruby-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-138">UWP</span><span class="sxs-lookup"><span data-stu-id="b3a9a-138">UWP</span></span></td>
    <td><span data-ttu-id="b3a9a-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-139">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample/tree/last_v1_auth">REST sample</a>
    </span></span></td>     
    <td><span data-ttu-id="b3a9a-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">Exemplo de SDK</a> ou ¶<a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">Exemplo de REST</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-140">
        <a href="https://github.com/microsoftgraph/uwp-csharp-connect-sample">SDK sample</a> or <a href="https://github.com/microsoftgraph/uwp-csharp-connect-rest-sample">REST sample</a>
    </span></span></td> 
  </tr>
  <tr>
    <td><span data-ttu-id="b3a9a-141">Xamarin</span><span class="sxs-lookup"><span data-stu-id="b3a9a-141">Xamarin</span></span></td>
    <td>
    </td>     
    <td><span data-ttu-id="b3a9a-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">Exemplo de SDK</a>
    </span><span class="sxs-lookup"><span data-stu-id="b3a9a-142">
        <a href="https://github.com/microsoftgraph/xamarin-csharp-connect-sample">SDK sample</a>
    </span></span></td> 
  </tr>
</table>

## <a name="see-also"></a><span data-ttu-id="b3a9a-143">Ver também</span><span class="sxs-lookup"><span data-stu-id="b3a9a-143">See also</span></span>
- <span data-ttu-id="b3a9a-144">Experimente exemplos de chamada REST em nosso [Gerenciador de API](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="b3a9a-144">Try out sample REST calls in our [API Explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>
- [<span data-ttu-id="b3a9a-145">Documentação de ponto de extremidade do Azure AD</span><span class="sxs-lookup"><span data-stu-id="b3a9a-145">Azure AD endpoint documentation</span></span>](https://azure.microsoft.com/documentation/services/active-directory/)
- [<span data-ttu-id="b3a9a-146">Documentação de ponto de extremidade do Azure AD v2.0</span><span class="sxs-lookup"><span data-stu-id="b3a9a-146">Azure AD v2.0 endpoint documentation</span></span>](https://azure.microsoft.com/documentation/articles/?service=active-directory&term=azure+ad+v2.0)
