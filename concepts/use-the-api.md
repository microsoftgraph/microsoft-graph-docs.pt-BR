---
title: Usar a API do Microsoft Graph
description: O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você registrar seu aplicativo e obter tokens de autenticação para um usuário ou serviço, é possível fazer solicitações para a API do Microsoft Graph.
author: jackson-woods
ms.openlocfilehash: 6f319540853e94497c6553b1bd44f7a8d3a33575
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27340051"
---
# <a name="use-the-microsoft-graph-api"></a><span data-ttu-id="a754e-104">Usar a API do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="a754e-104">Use the Microsoft Graph API</span></span>

<span data-ttu-id="a754e-p102">O Microsoft Graph é uma API Web RESTful que permite que você acesse os recursos de serviço do Microsoft Cloud. Depois que você [registrar seu aplicativo](auth-register-app-v2.md) e [obter tokens de autenticação para um usuário](auth-v2-user.md) ou [serviço](auth-v2-service.md), é possível fazer solicitações para a API do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a754e-p102">Microsoft Graph is a RESTful web API that enables you to access Microsoft Cloud service resources. After you [register your app](auth-register-app-v2.md) and [get authentication tokens for a user](auth-v2-user.md) or [service](auth-v2-service.md), you can make requests to the Microsoft Graph API.</span></span>

> <span data-ttu-id="a754e-107">**Importante:**  a maneira como políticas de acesso condicional se aplicam ao Microsoft Graph está mudando.</span><span class="sxs-lookup"><span data-stu-id="a754e-107">**Important:**  How conditional access policies apply to Microsoft Graph is changing.</span></span> <span data-ttu-id="a754e-108">Os aplicativos precisam ser atualizados para lidar com cenários em que as políticas de acesso condicional são configuradas.</span><span class="sxs-lookup"><span data-stu-id="a754e-108">Applications need to be updated to handle scenarios where conditional access policies are configured.</span></span> <span data-ttu-id="a754e-109">Para obter mais informações e orientações, confira [Diretrizes de desenvolvedor para acesso condicional do Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span><span class="sxs-lookup"><span data-stu-id="a754e-109">For more information and guidance, see [Developer Guidance for Azure Active Directory Conditional Access](https://docs.microsoft.com/azure/active-directory/develop/active-directory-conditional-access-developer).</span></span>

<span data-ttu-id="a754e-110">Para ler de ou gravar em um recurso como um usuário ou uma mensagem de email, você constrói uma solicitação semelhante ao seguinte.</span><span class="sxs-lookup"><span data-stu-id="a754e-110">To read from or write to a resource such as a user or an email message, you construct a request that looks like the following.</span></span>

```http
https://graph.microsoft.com/{version}/{resource}?query-parameters
```

<span data-ttu-id="a754e-111">Os componentes de uma solicitação incluem:</span><span class="sxs-lookup"><span data-stu-id="a754e-111">The components of a request include:</span></span>

* <span data-ttu-id="a754e-112">[Método HTTP](#http-methods) -o método HTTP usado na solicitação para o Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="a754e-112">[HTTP method](#http-methods) - The HTTP method used on the request to Microsoft Graph.</span></span>
* <span data-ttu-id="a754e-113">[`{version}`](#version) – a versão da API do Microsoft Graph que seu aplicativo está usando.</span><span class="sxs-lookup"><span data-stu-id="a754e-113">[`{version}`](#version) - The version of the Microsoft Graph API your application is using.</span></span>
* <span data-ttu-id="a754e-114">[`{resource}`](#resource) – o recurso no Microsoft Graph ao qual você está fazendo referência.</span><span class="sxs-lookup"><span data-stu-id="a754e-114">[`{resource}`](#resource) - The resource in Microsoft Graph that you're referencing.</span></span>
* <span data-ttu-id="a754e-115">[query-parameters](#query-parameters-optional) – um conjunto opcional de parâmetros para modificar a solicitação ou a resposta.</span><span class="sxs-lookup"><span data-stu-id="a754e-115">[query-parameters](#query-parameters-optional) - An optional set of parameters to modify the request or response.</span></span>

<span data-ttu-id="a754e-116">Depois de fazer uma solicitação, uma resposta é retornada, que inclui:</span><span class="sxs-lookup"><span data-stu-id="a754e-116">After you make a request, a response is returned that includes:</span></span> 

* <span data-ttu-id="a754e-p104">Código de status – um código de status HTTP que indica o sucesso ou o fracasso. Para obter detalhes sobre os códigos de erro HTTP, confira [Erros](errors.md).</span><span class="sxs-lookup"><span data-stu-id="a754e-p104">Status code - An HTTP status code that indicates success or failure. For details about HTTP error codes, see [Errors](errors.md).</span></span>
* <span data-ttu-id="a754e-p105">Mensagem de resposta – os dados que você solicitou ou o resultado da operação. A mensagem de resposta pode estar vazia em algumas operações.</span><span class="sxs-lookup"><span data-stu-id="a754e-p105">Response message - The data that you requested or the result of the operation. The response message can be empty for some operations.</span></span>
* <span data-ttu-id="a754e-p106">Link **Avançar** – se a solicitação retornar muitos dados, será necessário percorrê-los escolhendo **Avançar**. Para obter detalhes, confira [Paginação](paging.md).</span><span class="sxs-lookup"><span data-stu-id="a754e-p106">**Next** link - If your request returns a lot of data, you need to page through it by choosing **Next**. For details, see [Paging](paging.md).</span></span>

## <a name="http-methods"></a><span data-ttu-id="a754e-123">Métodos HTTP</span><span class="sxs-lookup"><span data-stu-id="a754e-123">HTTP methods</span></span>

<span data-ttu-id="a754e-p107">O Microsoft Graph usa o método HTTP em sua solicitação para determinar sua solicitação está fazendo. A API é compatível com os seguintes métodos.</span><span class="sxs-lookup"><span data-stu-id="a754e-p107">Microsoft Graph uses the HTTP method on your request to determine what your request is doing. The API supports the following methods.</span></span>


|<span data-ttu-id="a754e-126">**Method**</span><span class="sxs-lookup"><span data-stu-id="a754e-126">**Method**</span></span> |<span data-ttu-id="a754e-127">**Descrição**</span><span class="sxs-lookup"><span data-stu-id="a754e-127">**Description**</span></span>                             |
| :----- | :------------------------------------------- |
| <span data-ttu-id="a754e-128">GET</span><span class="sxs-lookup"><span data-stu-id="a754e-128">GET</span></span>    | <span data-ttu-id="a754e-129">Ler dados de um recurso.</span><span class="sxs-lookup"><span data-stu-id="a754e-129">Read data from a resource.</span></span>                   |
| <span data-ttu-id="a754e-130">POST</span><span class="sxs-lookup"><span data-stu-id="a754e-130">POST</span></span>   | <span data-ttu-id="a754e-131">Criar um novo recurso, ou executar uma ação.</span><span class="sxs-lookup"><span data-stu-id="a754e-131">Create a new resource, or perform an action.</span></span> |
| <span data-ttu-id="a754e-132">PATCH</span><span class="sxs-lookup"><span data-stu-id="a754e-132">PATCH</span></span>  | <span data-ttu-id="a754e-133">Atualizar um recurso com novos valores.</span><span class="sxs-lookup"><span data-stu-id="a754e-133">Update a resource with new values.</span></span>           |
| <span data-ttu-id="a754e-134">PUT</span><span class="sxs-lookup"><span data-stu-id="a754e-134">PUT</span></span>    | <span data-ttu-id="a754e-135">Substituir um recurso por um novo.</span><span class="sxs-lookup"><span data-stu-id="a754e-135">Replace a resource with a new one.</span></span>           |
| <span data-ttu-id="a754e-136">DELETE</span><span class="sxs-lookup"><span data-stu-id="a754e-136">DELETE</span></span> | <span data-ttu-id="a754e-137">Remover um recurso.</span><span class="sxs-lookup"><span data-stu-id="a754e-137">Remove a resource.</span></span>                           |

* <span data-ttu-id="a754e-138">Nos métodos **GET** e **DELETE**, nenhum corpo de solicitação é obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a754e-138">For the methods **GET** and **DELETE**, no request body is required.</span></span>
* <span data-ttu-id="a754e-139">Os métodos **POST**, **PATCH** e **PUT** precisam de um corpo de solicitação, normalmente especificado em formato JSON que contém informações adicionais, como os valores das propriedades do recurso.</span><span class="sxs-lookup"><span data-stu-id="a754e-139">The **POST**, **PATCH**, and **PUT** methods require a request body, usually specified in JSON format, that contains additional information, such as the values for properties of the resource.</span></span>

## <a name="version"></a><span data-ttu-id="a754e-140">Versão</span><span class="sxs-lookup"><span data-stu-id="a754e-140">Version</span></span>

<span data-ttu-id="a754e-141">O Microsoft Graph atualmente é compatível com duas versões: `v1.0` e `beta`.</span><span class="sxs-lookup"><span data-stu-id="a754e-141">Microsoft Graph currently supports two versions: `v1.0` and `beta`.</span></span>

* <span data-ttu-id="a754e-p108">O `v1.0` inclui APIs normalmente disponíveis. Use a versão 1.0 para todos os aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a754e-p108">`v1.0` includes generally available APIs. Use the v1.0 version for all production apps.</span></span>
* <span data-ttu-id="a754e-p109">O `beta` inclui APIs que estão atualmente em modo de visualização. Como podemos apresentar alterações significativas a nossas APIs beta, recomendamos que você use a versão beta apenas para testar aplicativos em desenvolvimento. Não use APIs beta em seus aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a754e-p109">`beta` includes APIs that are currently in preview. Because we might introduce breaking changes to our beta APIs, we recommend that you use the beta version only to test apps that are in development; do not use beta APIs in your production apps.</span></span>

<span data-ttu-id="a754e-p110">Estamos sempre buscando comentários sobre nossas APIs beta. Para fornecer comentários ou solicitar recursos, veja nossa página [UserVoice](https://officespdev.uservoice.com/).</span><span class="sxs-lookup"><span data-stu-id="a754e-p110">We are always looking for feedback on our beta APIs. To provide feedback or request features, see our [UserVoice](https://officespdev.uservoice.com/) page.</span></span>

<span data-ttu-id="a754e-148">Para saber mais sobre as versões da API, veja [Suporte e controle de versão](versioning-and-support.md).</span><span class="sxs-lookup"><span data-stu-id="a754e-148">For more information about API versions, see [Versioning and support](versioning-and-support.md).</span></span>

## <a name="resource"></a><span data-ttu-id="a754e-149">Resource</span><span class="sxs-lookup"><span data-stu-id="a754e-149">Resource</span></span>

<span data-ttu-id="a754e-p111">Sua URL incluirá um ou mais recursos com que você está interagindo na solicitação, como `me`, `users`, `groups`, `drives` e `sites`. Cada um dos recursos de nível superior também inclui **relações**, que podem ser usados para acessar recursos adicionais, como `me/messages` ou `me/drive`. Você também pode interagir com os recursos usando **métodos**, por exemplo, para enviar um email, use `me/sendMail`.</span><span class="sxs-lookup"><span data-stu-id="a754e-p111">Your URL will include the resource or resources you are interacting with in the request, such as `me`, `users`, `groups`, `drives`, and `sites`. Each of the top-level resources also include **relationships**, which you can use to access additional resources, like `me/messages` or `me/drive`. You can also interact with resources using **methods**; for example, to send an email, use `me/sendMail`.</span></span>

<span data-ttu-id="a754e-153">Para saber mais sobre como navegar por métodos e relações do recurso, confira [Desviar o gráfico](traverse-the-graph.md).</span><span class="sxs-lookup"><span data-stu-id="a754e-153">For more information about how to navigate resource relationships and methods, see [Traverse the graph](traverse-the-graph.md).</span></span> 

<span data-ttu-id="a754e-p112">Cada recurso pode exigir diferentes permissões de acesso. Muitas vezes será necessário um nível mais alto de permissões para criar ou atualizar um recurso do que para lê-lo. Para obter detalhes sobre as permissões necessárias, veja o tópico de referência do método.</span><span class="sxs-lookup"><span data-stu-id="a754e-p112">Each resource might require different permissions to access it. You will often need a higher level of permissions to create or update a resource than to read it. For details about required permissions, see the method reference topic.</span></span> 

<span data-ttu-id="a754e-157">Para obter detalhes sobre permissões, veja [Referência de permissões](permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="a754e-157">For details about permissions, see [Permissions reference](permissions-reference.md).</span></span>

## <a name="query-parameters-optional"></a><span data-ttu-id="a754e-158">Parâmetros de consulta (opcional)</span><span class="sxs-lookup"><span data-stu-id="a754e-158">Query parameters (optional)</span></span>

<span data-ttu-id="a754e-p113">Você pode usar parâmetros de consulta opcionais para personalizar a resposta em seu aplicativo Microsoft Graph. Use parâmetros de consulta para incluir mais ou menos propriedades do que a resposta padrão, filtrar a resposta para itens que correspondem a uma consulta personalizada ou oferecem parâmetros adicionais para um método.</span><span class="sxs-lookup"><span data-stu-id="a754e-p113">You can use optional query parameters to customize the response in your Microsoft Graph app. Use query parameters to include more or fewer properties than the default response, filter the response for items that match a custom query, or provide additional parameters for a method.</span></span>

<span data-ttu-id="a754e-161">Por exemplo, adicionar o seguinte parâmetro de filtro restringe as mensagens retornadas para apenas aquelas com a propriedade `emailAddress` de `jon@contoso.com`.</span><span class="sxs-lookup"><span data-stu-id="a754e-161">For example, adding the following filter parameter restricts the messages returned to only those with the `emailAddress` property of `jon@contoso.com`.</span></span>

```http
https://graph.microsoft.com/v1.0/me/messages?filter=emailAddress eq 'jon@contoso.com'
```

<span data-ttu-id="a754e-162">Para saber mais sobre os parâmetros de consulta, veja [Personalizar respostas](query-parameters.md).</span><span class="sxs-lookup"><span data-stu-id="a754e-162">For more information about query parameters, see [Customize responses](query-parameters.md).</span></span>

## <a name="next-steps"></a><span data-ttu-id="a754e-163">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="a754e-163">Next steps</span></span>

<span data-ttu-id="a754e-p114">Você está pronto para começar a trabalhar com o Microsoft Graph. Para saber mais, vá para o [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) para experimentar algumas solicitações, tente o [Início Rápido](https://developer.microsoft.com/graph/quick-start) ou comece a usar um dos nossos [SDKs e exemplos de código](https://developer.microsoft.com/graph/code-samples-and-sdks).</span><span class="sxs-lookup"><span data-stu-id="a754e-p114">You're ready to get up and running with Microsoft Graph. To learn more, go to the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) to try out some requests, try the [Quick Start](https://developer.microsoft.com/graph/quick-start), or get started using one of our [SDKs and code samples](https://developer.microsoft.com/graph/code-samples-and-sdks).</span></span>
