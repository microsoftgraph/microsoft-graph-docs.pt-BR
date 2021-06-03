---
title: Usar a API do Microsoft Graph
description: O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você registrar seu aplicativo e obter tokens de autenticação para um usuário ou serviço, é possível fazer solicitações para a API do Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: 1a478adb9053face3537a445e25dd69a908b2525
ms.sourcegitcommit: 91d8454bfff853905e3a5e86623fcb06931507ed
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/03/2021
ms.locfileid: "52732144"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="1918c-104">Usar a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1918c-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="1918c-p102">O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você [registrar seu aplicativo](auth-register-app-v2.md) e [obter tokens de autenticação para um usuário](auth-v2-user.md) ou [serviço](auth-v2-service.md), é possível fazer solicitações para a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1918c-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="1918c-107">**Importante:**  a maneira como políticas de acesso condicional se aplicam ao Microsoft Graph está mudando.</span><span class="sxs-lookup"><span data-stu-id="1918c-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="1918c-108">Os aplicativos precisam ser atualizados para lidar com cenários em que as políticas de acesso condicional são configuradas.</span><span class="sxs-lookup"><span data-stu-id="1918c-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="1918c-109">Para obter mais informações e orientações, confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="1918c-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

## <a name="odata-namespace"></a><span data-ttu-id="1918c-110">Espaço de nomes (namespace) OData</span><span class="sxs-lookup"><span data-stu-id="1918c-110">OData namespace</span></span>

<span data-ttu-id="1918c-111">A API do Microsoft Graph define a maioria dos seus recursos, métodos e enumerações no namespace OData, `microsoft.graph`nos [metadados do Microsoft Graph](traverse-the-graph.md#microsoft-graph-api-metadata).</span><span class="sxs-lookup"><span data-stu-id="1918c-111">The Microsoft Graph API defines most of its resources, methods, and enumerations in the OData namespace, `microsoft.graph`, in the [Microsoft Graph metadata](traverse-the-graph.md#microsoft-graph-api-metadata).</span></span> <span data-ttu-id="1918c-112">Um pequeno número de conjuntos de APIs são definidos em seus subnamespaces, como a [API de registros de chamada](/graph/api/resources/callrecords-api-overview), que define recursos como [callRecord](/graph/api/resources/callrecords-callrecord) no `microsoft.graph.callRecords`.</span><span class="sxs-lookup"><span data-stu-id="1918c-112">A small number of API sets are defined in their sub-namespaces, such as the [call records API](/graph/api/resources/callrecords-api-overview) which defines resources like [callRecord](/graph/api/resources/callrecords-callrecord) in `microsoft.graph.callRecords`.</span></span> 

<span data-ttu-id="1918c-113">A menos que especificado explicitamente no tópico correspondente, considere tipos, métodos e enumerações fazem parte do espaço de nomes `microsoft.graph`.</span><span class="sxs-lookup"><span data-stu-id="1918c-113">Unless explicitly specified in the corresponding topic, assume types, methods, and enumerations are part of the `microsoft.graph` namespace.</span></span>

## <a name="call-a-rest-api-method"></a><span data-ttu-id="1918c-114">Método de chamada à API REST</span><span class="sxs-lookup"><span data-stu-id="1918c-114">Call a REST API method</span></span>

<span data-ttu-id="1918c-115">Para ler de ou gravar em um recurso como um usuário ou uma mensagem de email, você constrói uma solicitação semelhante ao visto abaixo:</span><span class="sxs-lookup"><span data-stu-id="1918c-115">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="1918c-116">Os componentes de uma solicitação incluem:</span><span class="sxs-lookup"><span data-stu-id="1918c-116">The components of a request include:</span></span>

* <span data-ttu-id="1918c-117">[{Método HTTP}](#http-methods) – O método HTTP usado na solicitação para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1918c-117">[{HTTP method}](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="1918c-118">[{versão}](#version) – A versão da API do Microsoft Graph que seu aplicativo está usando.</span><span class="sxs-lookup"><span data-stu-id="1918c-118">[{version}](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="1918c-119">[{recurso}](#resource) – O recurso no Microsoft Graph ao qual você está fazendo referência.</span><span class="sxs-lookup"><span data-stu-id="1918c-119">[{resource}](#resource) - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="1918c-120">[{Parâmetros-da-consultas}](#query-parameters) –Opções de consulta OData opcionais ou parâmetros do método REST que personalizam a resposta.</span><span class="sxs-lookup"><span data-stu-id="1918c-120">[{query-parameters}](#query-parameters) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="1918c-121">Depois de fazer uma solicitação, uma resposta é retornada, que inclui:</span><span class="sxs-lookup"><span data-stu-id="1918c-121">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="1918c-p105">Código de status – um código de status HTTP que indica o sucesso ou o fracasso. Para obter detalhes sobre os códigos de erro HTTP, confira [Erros](errors.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-p105">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="1918c-p106">Mensagem de resposta – os dados que você solicitou ou o resultado da operação. A mensagem de resposta pode estar vazia em algumas operações.</span><span class="sxs-lookup"><span data-stu-id="1918c-p106">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="1918c-p107">`nextLink` – Se a solicitação retornar muitos dados, será necessário percorrê-los usando a URL retornada no `@odata.nextLink`. Para obter detalhes, confira [Paginação](paging.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-p107">`nextLink` - If your request returns a lot of data, you need to page through it by using the URL returned in `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="1918c-128">Métodos HTTP</span><span class="sxs-lookup"><span data-stu-id="1918c-128">HTTP methods</span></span>

<span data-ttu-id="1918c-p108">O Microsoft Graph usa o método HTTP em sua solicitação para determinar sua solicitação está fazendo. A API é compatível com os seguintes métodos.</span><span class="sxs-lookup"><span data-stu-id="1918c-p108">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>

|<span data-ttu-id="1918c-131">**Method**</span><span class="sxs-lookup"><span data-stu-id="1918c-131">**Method**</span></span> |<span data-ttu-id="1918c-132">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="1918c-132">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="1918c-133">GET</span><span class="sxs-lookup"><span data-stu-id="1918c-133">GET</span></span>    | <span data-ttu-id="1918c-134">Ler dados de um recurso.</span><span class="sxs-lookup"><span data-stu-id="1918c-134">Read data from a resource.</span></span>                   |
| <span data-ttu-id="1918c-135">POST</span><span class="sxs-lookup"><span data-stu-id="1918c-135">POST</span></span>   | <span data-ttu-id="1918c-136">Criar um novo recurso, ou executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="1918c-136">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="1918c-137">PATCH</span><span class="sxs-lookup"><span data-stu-id="1918c-137">PATCH</span></span>  | <span data-ttu-id="1918c-138">Atualizar um recurso com novos valores.</span><span class="sxs-lookup"><span data-stu-id="1918c-138">Update a resource with new values.</span></span>           |
| <span data-ttu-id="1918c-139">PUT</span><span class="sxs-lookup"><span data-stu-id="1918c-139">PUT</span></span>    | <span data-ttu-id="1918c-140">Substituir um recurso por um novo.</span><span class="sxs-lookup"><span data-stu-id="1918c-140">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="1918c-141">DELETE</span><span class="sxs-lookup"><span data-stu-id="1918c-141">DELETE</span></span> | <span data-ttu-id="1918c-142">Remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="1918c-142">Remove a resource.</span></span>                           |

* <span data-ttu-id="1918c-143">Nos métodos CRUD, `GET` e `DELETE`, nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1918c-143">For the CRUD methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="1918c-144">Os métodos `POST`, `PATCH` e `PUT` precisam de um corpo de solicitação, normalmente especificado em formato JSON que contém informações adicionais, como os valores das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="1918c-144">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="1918c-145">Versão</span><span class="sxs-lookup"><span data-stu-id="1918c-145">Version</span></span>

<span data-ttu-id="1918c-146">O Microsoft Graph atualmente é compatível com duas versões: `v1.0` e `beta`.</span><span class="sxs-lookup"><span data-stu-id="1918c-146">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="1918c-p109">O `v1.0` inclui APIs normalmente disponíveis. Use a versão 1.0 para todos os aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1918c-p109">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="1918c-p110">O `beta` inclui APIs que estão atualmente em modo de visualização. Como podemos apresentar alterações significativas a nossas APIs beta, recomendamos que você use a versão beta apenas para testar aplicativos em desenvolvimento. Não use APIs beta em seus aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1918c-p110">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="1918c-p111">Estamos sempre buscando comentários sobre nossas APIs beta. Para enviar comentários ou solicitar recursos, confira nossa página [fórum de ideias da plataforma de desenvolvedores do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span><span class="sxs-lookup"><span data-stu-id="1918c-p111">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [Microsoft 365 Developer Platform ideas forum](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).</span></span>

<span data-ttu-id="1918c-153">Para saber mais sobre as versões da API, veja [Suporte e controle de versão](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-153">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="1918c-154">Recurso</span><span class="sxs-lookup"><span data-stu-id="1918c-154">Resource</span></span>

<span data-ttu-id="1918c-155">Um recurso pode ser uma entidade ou tipo complexo, normalmente definido com propriedades.</span><span class="sxs-lookup"><span data-stu-id="1918c-155">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="1918c-156">As entidades são diferentes de tipos complexos, incluindo sempre uma propriedade de **id**.</span><span class="sxs-lookup"><span data-stu-id="1918c-156">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="1918c-p113">Sua URL incluirá um ou mais recursos com os quais você está interagindo, como `me`, **usuário**, **grupo**, **unidade** e **site**. Muitas vezes, os recursos de nível superior também incluem _relações_, que você pode usar para acessar recursos adicionais, como `me/messages` ou `me/drive`. Você também pode interagir com os recursos usando _métodos_; para enviar um email, use `me/sendMail`. Para obter mais informações, confira [Acessar dados e métodos navegando no Microsoft Graph](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-p113">Your URL will include the resource you are interacting with in the request, such as `me`, **user**, **group**, **drive**, and **site**. Often, top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`. You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`. For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="1918c-p114">Cada recurso pode exigir diferentes permissões de acesso. Muitas vezes será necessário um nível mais alto de permissões para criar ou atualizar um recurso do que para lê-lo. Para obter detalhes sobre as permissões necessárias, veja o tópico de referência do método.</span><span class="sxs-lookup"><span data-stu-id="1918c-p114">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="1918c-164">Para obter detalhes sobre permissões, veja [Referência de permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-164">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="1918c-165">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="1918c-165">Query parameters</span></span>

<span data-ttu-id="1918c-166">Os parâmetros de consulta podem ser opções de consulta do sistema OData ou outras cadeias de caracteres que um método aceita para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="1918c-166">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="1918c-167">Use parâmetros de consulta do sistema OData para incluir mais ou menos propriedades do que a resposta padrão, filtrar a resposta para itens que correspondem a uma consulta personalizada ou oferecem parâmetros adicionais para um método.</span><span class="sxs-lookup"><span data-stu-id="1918c-167">You can use optional OData system query options to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="1918c-168">Por exemplo, adicionar o seguinte parâmetro de `filter` restringe as mensagens retornadas para apenas aquelas com a propriedade de `emailAddress` do `jon@contoso.com`. </span><span class="sxs-lookup"><span data-stu-id="1918c-168">For example, adding the following `filter` parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="1918c-169">Para obter mais informações sobre as opções de consulta OData, confira [Usar parâmetros de consulta para personalizar respostas](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-169">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="1918c-170">Com exceção das opções de consulta OData, alguns métodos exigem valores de parâmetro especificados como parte da URL da consulta.</span><span class="sxs-lookup"><span data-stu-id="1918c-170">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="1918c-171">Por exemplo, é possível obter uma coleção de eventos ocorridos durante um período de tempo no calendário de um usuário, consultando a relação **calendarView** de um **usuário** e especificando o período dos valores `startDateTime` e `endDateTime` como parâmetros da consulta:</span><span class="sxs-lookup"><span data-stu-id="1918c-171">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="tools-for-interacting-with-microsoft-graph"></a><span data-ttu-id="1918c-172">Ferramentas para interagir com o Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="1918c-172">Tools for interacting with Microsoft Graph</span></span>

### <a name="graph-explorer"></a><span data-ttu-id="1918c-173">Explorador do Graph</span><span class="sxs-lookup"><span data-stu-id="1918c-173">Graph Explorer</span></span>

<span data-ttu-id="1918c-p116">O Explorador do Graph é uma ferramenta baseada na Web que você pode usar para criar e testar solicitações usando as APIs do Microsoft Graph. Você pode acessar o Explorador do Graph em: [https://developer.microsoft.com/graph/graph-explorer](https://developer.microsoft.com/graph/graph-explorer).</span><span class="sxs-lookup"><span data-stu-id="1918c-p116">Graph Explorer is a web-based tool that you can use to build and test requests using Microsoft Graph APIs. You can access Graph Explorer at: [https://developer.microsoft.com/graph/graph-explorer](https://developer.microsoft.com/graph/graph-explorer).</span></span>

<span data-ttu-id="1918c-p117">Você pode acessar os dados de demonstração sem fazer logon, ou pode fazer logon em um locatário de sua preferência. Use as etapas a seguir para criar a solicitação:</span><span class="sxs-lookup"><span data-stu-id="1918c-p117">You can either access demo data without signing in, or you can sign in to a tenant of your own. Use the following steps to build the request:</span></span>

1. <span data-ttu-id="1918c-178">Selecione o método HTTP.</span><span class="sxs-lookup"><span data-stu-id="1918c-178">Select the HTTP method.</span></span>
2. <span data-ttu-id="1918c-179">Selecione a versão da API que você deseja usar.</span><span class="sxs-lookup"><span data-stu-id="1918c-179">Select the version of API that you want to use.</span></span>
3. <span data-ttu-id="1918c-180">Digite a consulta na caixa de texto da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1918c-180">Type the query in the request text box.</span></span>
4. <span data-ttu-id="1918c-181">Selecione **Executar consulta**.</span><span class="sxs-lookup"><span data-stu-id="1918c-181">Select **Run Query**.</span></span> 

<span data-ttu-id="1918c-182">O exemplo a seguir mostra uma solicitação que retorna informações sobre usuários no locatário da demonstração:</span><span class="sxs-lookup"><span data-stu-id="1918c-182">The following example shows a request that returns information about users in the demo tenant:</span></span>

![Captura de tela do Explorador do Graph com uma solicitação de usuário GET realçada](./images/graph-explorer.png)

<span data-ttu-id="1918c-184">Os exemplos de consultas são fornecidos no Explorador do Graph para permitir que você execute solicitações comuns mais rapidamente.</span><span class="sxs-lookup"><span data-stu-id="1918c-184">Sample queries are provided in Graph Explorer to enable you to more quickly run common requests.</span></span> <span data-ttu-id="1918c-185">Para ver os exemplos disponíveis, selecione **mostrar mais exemplos**.</span><span class="sxs-lookup"><span data-stu-id="1918c-185">To see the samples that are available, select **show more samples**.</span></span> <span data-ttu-id="1918c-186">Selecione **Ativado** para o conjunto de exemplos que deseja ver e, depois de fechar a janela de seleção, você deverá ver uma lista de solicitações predefinidas.</span><span class="sxs-lookup"><span data-stu-id="1918c-186">Select **On** for the set of samples that you want to see, and then after closing the selection window, you should see a list of predefined requests.</span></span>

<span data-ttu-id="1918c-187">Um código de status e uma mensagem são exibidos depois que uma solicitação é enviada, e a resposta é exibida na guia **Visualização de resposta**.</span><span class="sxs-lookup"><span data-stu-id="1918c-187">A status code and message are displayed after a request is sent and the response is shown in the **Response Preview** tab.</span></span>

### <a name="postman"></a><span data-ttu-id="1918c-188">Postman</span><span class="sxs-lookup"><span data-stu-id="1918c-188">Postman</span></span>

<span data-ttu-id="1918c-189">O Postman é uma ferramenta que você pode usar para criar e testar solicitações usando as APIs do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1918c-189">Postman is a tool that you can use to build and test requests using the Microsoft Graph APIs.</span></span> <span data-ttu-id="1918c-190">Você pode baixar o Postman em: [https://www.getpostman.com/](https://www.getpostman.com/).</span><span class="sxs-lookup"><span data-stu-id="1918c-190">You can download Postman at: [https://www.getpostman.com/](https://www.getpostman.com/).</span></span> <span data-ttu-id="1918c-191">Para interagir com o Microsoft Graph no Postman, use a coleção do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="1918c-191">To interact with Microsoft Graph in Postman, you use the Microsoft Graph collection.</span></span>

<span data-ttu-id="1918c-192">Para obter mais informações, confira [Usar o Postman com a API do Microsoft Graph](./use-postman.md).</span><span class="sxs-lookup"><span data-stu-id="1918c-192">For more information, see [Use Postman with the Microsoft Graph API](./use-postman.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="1918c-193">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1918c-193">Next steps</span></span>

<span data-ttu-id="1918c-p120">Você está pronto para começar a usar o Microsoft Graph. Experimente o [Início rápido](https://developer.microsoft.com/graph/quick-start) ou comece usando um de nossos [SDKs e exemplos de código](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="1918c-p120">You're ready to get up and running with Microsoft Graph. Try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
