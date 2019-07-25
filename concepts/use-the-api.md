---
title: Usar a API do Microsoft Graph
description: O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você registrar seu aplicativo e obter tokens de autenticação para um usuário ou serviço, é possível fazer solicitações para a API do Microsoft Graph.
author: jackson-woods
localization_priority: Priority
ms.openlocfilehash: 18de281cc0becfacfdabe5fb81a68358f04c3747
ms.sourcegitcommit: 8844023e15b7649a5c03603aee243acf85930ef2
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/24/2019
ms.locfileid: "35840639"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="2c690-104">Usar a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="2c690-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="2c690-p102">O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você [registrar seu aplicativo](auth-register-app-v2.md) e [obter tokens de autenticação para um usuário](auth-v2-user.md) ou [serviço](auth-v2-service.md), é possível fazer solicitações para a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c690-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="2c690-107">**Importante:**  a maneira como políticas de acesso condicional se aplicam ao Microsoft Graph está mudando.</span><span class="sxs-lookup"><span data-stu-id="2c690-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="2c690-108">Os aplicativos precisam ser atualizados para lidar com cenários em que as políticas de acesso condicional são configuradas.</span><span class="sxs-lookup"><span data-stu-id="2c690-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="2c690-109">Para obter mais informações e orientações, confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="2c690-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="2c690-110">Para ler de ou gravar em um recurso como um usuário ou uma mensagem de email, você constrói uma solicitação semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="2c690-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
{HTTP method} https://graph.microsoft.com/{version}/{resource}?{query-parameters}
```

<span data-ttu-id="2c690-111">Os componentes de uma solicitação incluem:</span><span class="sxs-lookup"><span data-stu-id="2c690-111">The components of a request include:</span></span>

* <span data-ttu-id="2c690-112">[{Método HTTP}](#http-methods) – O método HTTP usado na solicitação para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="2c690-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="2c690-113">[{versão}](#version) – A versão da API do Microsoft Graph que seu aplicativo está usando.</span><span class="sxs-lookup"><span data-stu-id="2c690-113">   - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="2c690-114">[{recurso}](#resource) – O recurso no Microsoft Graph ao qual você está fazendo referência.</span><span class="sxs-lookup"><span data-stu-id="2c690-114">   - The resource in Microsoft Graph that you're referencing.</span></span> 
* <span data-ttu-id="2c690-115">[{Parâmetros-da-consultas}](#query-parameters-optional) –Opções de consulta OData opcionais ou parâmetros do método REST que personalizam a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c690-115">[{query-parameters}](#query-parameters-optional) - Optional OData query options or REST method parameters that customize the response.</span></span>

<span data-ttu-id="2c690-116">Depois de fazer uma solicitação, uma resposta é retornada, que inclui:</span><span class="sxs-lookup"><span data-stu-id="2c690-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="2c690-p104">Código de status – um código de status HTTP que indica o sucesso ou o fracasso. Para obter detalhes sobre os códigos de erro HTTP, confira [Erros](errors.md).</span><span class="sxs-lookup"><span data-stu-id="2c690-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="2c690-p105">Mensagem de resposta – os dados que você solicitou ou o resultado da operação. A mensagem de resposta pode estar vazia em algumas operações.</span><span class="sxs-lookup"><span data-stu-id="2c690-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="2c690-p106">`nextLink` – Se a solicitação retornar muitos dados, será necessário percorrê-los usando a URL retornada no `@odata.nextLink`. Para obter detalhes, confira [Paginação](paging.md).</span><span class="sxs-lookup"><span data-stu-id="2c690-p106">`nextLink` link - If your request returns a lot of data, you need to page through it by choosing `@odata.nextLink`. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="2c690-123">Métodos HTTP</span><span class="sxs-lookup"><span data-stu-id="2c690-123">HTTP methods</span></span>

<span data-ttu-id="2c690-p107">O Microsoft Graph usa o método HTTP em sua solicitação para determinar sua solicitação está fazendo. A API é compatível com os seguintes métodos.</span><span class="sxs-lookup"><span data-stu-id="2c690-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="2c690-126">**Method**</span><span class="sxs-lookup"><span data-stu-id="2c690-126">**Method**</span></span> |<span data-ttu-id="2c690-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="2c690-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="2c690-128">GET</span><span class="sxs-lookup"><span data-stu-id="2c690-128">GET</span></span>    | <span data-ttu-id="2c690-129">Ler dados de um recurso.</span><span class="sxs-lookup"><span data-stu-id="2c690-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="2c690-130">POST</span><span class="sxs-lookup"><span data-stu-id="2c690-130">POST</span></span>   | <span data-ttu-id="2c690-131">Criar um novo recurso, ou executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="2c690-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="2c690-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="2c690-132">PATCH</span></span>  | <span data-ttu-id="2c690-133">Atualizar um recurso com novos valores.</span><span class="sxs-lookup"><span data-stu-id="2c690-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="2c690-134">PUT</span><span class="sxs-lookup"><span data-stu-id="2c690-134">PUT</span></span>    | <span data-ttu-id="2c690-135">Substituir um recurso por um novo.</span><span class="sxs-lookup"><span data-stu-id="2c690-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="2c690-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="2c690-136">DELETE</span></span> | <span data-ttu-id="2c690-137">Remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="2c690-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="2c690-138">Nos métodos CRUD, `GET` e `DELETE`, nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2c690-138">For the methods `GET` and `DELETE`, no request body is required.</span></span>
* <span data-ttu-id="2c690-139">Os métodos `POST`, `PATCH` e `PUT` precisam de um corpo de solicitação, normalmente especificado em formato JSON que contém informações adicionais, como os valores das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="2c690-139">The `POST`, `PATCH`, and `PUT` methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="2c690-140">Versão</span><span class="sxs-lookup"><span data-stu-id="2c690-140">Version</span></span>

<span data-ttu-id="2c690-141">O Microsoft Graph atualmente é compatível com duas versões: `v1.0` e `beta`.</span><span class="sxs-lookup"><span data-stu-id="2c690-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="2c690-p108">O `v1.0` inclui APIs normalmente disponíveis. Use a versão 1.0 para todos os aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c690-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="2c690-p109">O `beta` inclui APIs que estão atualmente em modo de visualização. Como podemos apresentar alterações significativas a nossas APIs beta, recomendamos que você use a versão beta apenas para testar aplicativos em desenvolvimento. Não use APIs beta em seus aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2c690-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="2c690-p110">Estamos sempre buscando comentários sobre nossas APIs beta. Para fornecer comentários ou solicitar recursos, veja nossa página [UserVoice](https://officespdev.uservoice.com/).</span><span class="sxs-lookup"><span data-stu-id="2c690-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="2c690-148">Para saber mais sobre as versões da API, veja [Suporte e controle de versão](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="2c690-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="2c690-149">Recurso</span><span class="sxs-lookup"><span data-stu-id="2c690-149">Resource</span></span>

<span data-ttu-id="2c690-150">Um recurso pode ser uma entidade ou tipo complexo, normalmente definido com propriedades.</span><span class="sxs-lookup"><span data-stu-id="2c690-150">A resource can be an entity or complex type, commonly defined with properties.</span></span> <span data-ttu-id="2c690-151">As entidades são diferentes de tipos complexos, incluindo sempre uma propriedade de **id**.</span><span class="sxs-lookup"><span data-stu-id="2c690-151">Entities differ from complex types by always including an **id** property.</span></span>

<span data-ttu-id="2c690-152">Sua URL incluirá um ou mais recursos com que você está interagindo na solicitação, como `me`, **usuário**, **grupo**, **unidade** e **site**.</span><span class="sxs-lookup"><span data-stu-id="2c690-152">Your URL will include the resource or resources you are interacting with in the request, such as `me`, \*\*\*\*, \*\*\*\*, \*\*\*\*, and \*\*\*\*.</span></span> <span data-ttu-id="2c690-153">Frequentemente, cada um dos recursos de nível superior também inclui _relações_, que podem ser usadas para acessar recursos adicionais, como `me/messages` ou `me/drive`.</span><span class="sxs-lookup"><span data-stu-id="2c690-153">Each of the top-level resources also include _relationships_, which you can use to access additional resources, like `me/messages` or `me/drive`.</span></span> <span data-ttu-id="2c690-154">Você também pode interagir com os recursos usando _métodos_; por exemplo, para enviar um email, use `me/sendMail`.</span><span class="sxs-lookup"><span data-stu-id="2c690-154">You can also interact with resources using _methods_; for example, to send an email, use `me/sendMail`.</span></span> <span data-ttu-id="2c690-155">Para mais informações, confira [Acessar dados e métodos ao navegar no Microsoft Graph](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="2c690-155">For more information, see [Access data and methods by navigating Microsoft Graph](traverse-the-graph.md).</span></span>

<span data-ttu-id="2c690-p113">Cada recurso pode exigir diferentes permissões de acesso. Muitas vezes será necessário um nível mais alto de permissões para criar ou atualizar um recurso do que para lê-lo. Para obter detalhes sobre as permissões necessárias, veja o tópico de referência do método.</span><span class="sxs-lookup"><span data-stu-id="2c690-p113">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="2c690-159">Para obter detalhes sobre permissões, veja [Referência de permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="2c690-159">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters"></a><span data-ttu-id="2c690-160">Parâmetros de consulta</span><span class="sxs-lookup"><span data-stu-id="2c690-160">Query parameters</span></span>

<span data-ttu-id="2c690-161">Os parâmetros de consulta podem ser opções de consulta do sistema OData ou outras cadeias de caracteres que um método aceita para personalizar a resposta.</span><span class="sxs-lookup"><span data-stu-id="2c690-161">Query parameters can be OData system query options, or other strings that a method accepts to customize its response.</span></span>

<span data-ttu-id="2c690-162">Use parâmetros de consulta do sistema OData para incluir mais ou menos propriedades do que a resposta padrão, filtrar a resposta para itens que correspondem a uma consulta personalizada ou oferecem parâmetros adicionais para um método.</span><span class="sxs-lookup"><span data-stu-id="2c690-162">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="2c690-163">Por exemplo, adicionar o seguinte parâmetro de `filter` restringe as mensagens retornadas para apenas aquelas com a propriedade de `emailAddress` do `jon@contoso.com`. </span><span class="sxs-lookup"><span data-stu-id="2c690-163">For example, adding the following filter parameter restricts the messages returned to only those with the  property of .</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="2c690-164">Para obter mais informações sobre as opções de consulta OData, confira [Usar parâmetros de consulta para personalizar respostas](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="2c690-164">For more information about OData query options, see [Use query parameters to customize responses](query-parameters.md).</span></span>

<span data-ttu-id="2c690-165">Com exceção das opções de consulta OData, alguns métodos exigem valores de parâmetro especificados como parte da URL da consulta.</span><span class="sxs-lookup"><span data-stu-id="2c690-165">Aside from OData query options, some methods require parameter values specified as part of the query URL.</span></span> <span data-ttu-id="2c690-166">Por exemplo, é possível obter uma coleção de eventos ocorridos durante um período de tempo no calendário de um usuário, consultando a relação **calendarView** de um **usuário**e especificando o período dos valores `startDateTime` e `endDateTime` como parâmetros da consulta:</span><span class="sxs-lookup"><span data-stu-id="2c690-166">For example, you can get a collection of events that occurred during a time period in a user's calendar, by querying the **calendarView** relationship of a **user**, and specifying the period `startDateTime` and `endDateTime` values as query parameters:</span></span>

<!-- {
  "blockType": "ignored"
}-->
```http
GET https://graph.microsoft.com/me/calendarView?startDateTime=2019-09-01T09:00:00.0000000&endDateTime=2019-09-01T17:00:00.0000000
```

## <a name="next-steps"></a><span data-ttu-id="2c690-167">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="2c690-167">Next steps</span></span>

<span data-ttu-id="2c690-p115">Você está pronto para começar a trabalhar com o Microsoft Graph. Para saber mais, vá para o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para experimentar algumas solicitações, tente o [Início Rápido](https://developer.microsoft.com/graph/quick-start) ou comece a usar um dos nossos [SDKs e exemplos de código](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="2c690-p115">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
