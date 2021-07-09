---
title: Recursos avançados de consulta nos objetos do diretório Microsoft Azure Active Directory
description: Os objetos do diretório Microsoft Azure Active Directory suportam recursos avançados de consulta para acesso eficiente aos dados.
author: Licantrop0
localization_priority: Priority
ms.custom: graphiamtop20, scenarios:getting-started
ms.openlocfilehash: e8a6c4a3a2d37eafeaee85f7778baa68bad97357
ms.sourcegitcommit: 4888ac7504533344c4fc6828e2a06a002a1d72d3
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/09/2021
ms.locfileid: "53351283"
---
# <a name="advanced-query-capabilities-on-azure-ad-directory-objects"></a><span data-ttu-id="2f5ed-103">Recursos avançados de consulta nos objetos do diretório Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2f5ed-103">Advanced query capabilities on Azure AD directory objects</span></span>

<span data-ttu-id="2f5ed-104">Como o Microsoft Azure Active Directory continua a oferecer mais capacidades e melhorias na estabilidade, disponibilidade e desempenho, o Microsoft Graph também continua a evoluir e a escalar para acessar os dados de forma eficiente.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-104">As Azure AD continues to deliver more capabilities and improvements in stability, availability, and performance, Microsoft Graph also continues to evolve and scale to efficiently access the data.</span></span> <span data-ttu-id="2f5ed-105">Uma maneira é através do suporte crescente do Microsoft Graph para capacidades avançadas de consulta em vários objetos Microsoft Azure Active Directory e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-105">One way is through Microsoft Graph's increasing support for advanced query capabilities on various Azure AD objects and their properties.</span></span> <span data-ttu-id="2f5ed-106">Por exemplo, a adição de **Não** (`NOT`), **Não é igual a** (`ne`), e **Termina com** (`endsWith`) operadores no parâmetro `$filter` de consulta em outubro de 2020.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-106">For example, the addition of **Not** (`NOT`), **Not equals** (`ne`), and **Ends with** (`endsWith`) operators on the `$filter` query parameter in October 2020.</span></span>

<span data-ttu-id="2f5ed-107">O mecanismo de consulta do Microsoft Graph usa uma loja de índices para atender aos pedidos de consulta.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-107">The Microsoft Graph query engine uses an index store to fulfill query requests.</span></span> <span data-ttu-id="2f5ed-108">Para adicionar suporte para capacidades adicionais de consulta em algumas propriedades, estas propriedades são agora indexadas em um servidor separado.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-108">To add support for additional query capabilities on some properties, these properties are now indexed in a separate server.</span></span> <span data-ttu-id="2f5ed-109">Esta indexação separada permite que o MIcrosoft Azure Active Directory aumente o suporte e melhore o desempenho dos pedidos de consulta.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-109">This separate indexing allows Azure AD to increase support and improve the performance of the query requests.</span></span> <span data-ttu-id="2f5ed-110">Entretanto, estas capacidades avançadas de consulta não estão disponíveis por padrão, mas o solicitante também deve definir o **ConsistencyLevel** como `eventual` *e*, com exceção de `$search`, usar o parâmetro `$count` consulta (seja como [segmento URL](/graph/query-parameters#other-odata-url-capabilities) ou `$count=true` cadeia de caracteres).</span><span class="sxs-lookup"><span data-stu-id="2f5ed-110">However, these advanced query capabilities are not available by default but, the requestor must also set the **ConsistencyLevel** header set to `eventual` *and*, with the exception of `$search`, use the `$count` query parameter (either as a [URL segment](/graph/query-parameters#other-odata-url-capabilities) or `$count=true` query string).</span></span> <span data-ttu-id="2f5ed-111">O cabeçalho **ConsistencyLevel** e `$count` são referidos como *parâmetros de consulta avançados*.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-111">The **ConsistencyLevel** header and `$count` are referred to as *advanced query parameters*.</span></span>

<span data-ttu-id="2f5ed-112">Por exemplo, se você deseja recuperar apenas contas de usuários inativos, você pode executar qualquer uma destas consultas que utilizam o Parâmetro de consulta `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-112">For example, if you wish to retrieve only inactive user accounts, you can run either of these queries that use the `$filter` query parameter.</span></span>

+ <span data-ttu-id="2f5ed-113">Usar o parâmetro `$filter` consulta com o operador `eq`.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-113">Use the `$filter` query parameter with the `eq` operator.</span></span> <span data-ttu-id="2f5ed-114">Esta solicitação funcionará por padrão, ou seja, a solicitação não requer os parâmetros de consulta avançados.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-114">This request will work by default, that is, the request does not require the advanced query parameters.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_users_enabled"
} -->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/users?$filter=accountEnabled eq false
```

+ <span data-ttu-id="2f5ed-115">Usar o parâmetro `$filter` consulta com o operador `ne`.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-115">Use the `$filter` query parameter with the `ne` operator.</span></span> <span data-ttu-id="2f5ed-116">Esta solicitação não é suportada por padrão porque o `ne` operador só é suportado em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-116">This request is not supported by default because the `ne` operator is only supported in advanced queries.</span></span> <span data-ttu-id="2f5ed-117">Portanto, você deve adicionar o **ConsistencyLevel** cabeçalho para `eventual`*e* usar a `$count=true` cadeia de caracteres.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-117">Therefore, you must add the **ConsistencyLevel** header set to `eventual` *and* use the `$count=true` query string.</span></span>

<!-- {
  "blockType": "ignored",
  "name": "get_users_not_enabled"
} -->
```msgraph-interactive
https://graph.microsoft.com/v1.0/users?$filter=accountEnabled ne true&$count=true
ConsistencyLevel: eventual
```

<span data-ttu-id="2f5ed-118">Estes recursos avançados de consulta são suportados apenas em objetos Microsoft Azure Active Directory, ou seja, os seguintes recursos e suas relações que derivam do [directoryObject](/graph/api/resources/directoryobject):</span><span class="sxs-lookup"><span data-stu-id="2f5ed-118">These advanced query capabilities are supported only on Azure AD objects, that is, the following resources and their relationships that derive from [directoryObject](/graph/api/resources/directoryobject):</span></span>

- [<span data-ttu-id="2f5ed-119">aplicativo</span><span class="sxs-lookup"><span data-stu-id="2f5ed-119">application</span></span>](/graph/api/resources/application)
- [<span data-ttu-id="2f5ed-120">orgContact</span><span class="sxs-lookup"><span data-stu-id="2f5ed-120">orgContact</span></span>](/graph/api/resources/orgcontact)
- [<span data-ttu-id="2f5ed-121">device</span><span class="sxs-lookup"><span data-stu-id="2f5ed-121">device</span></span>](/graph/api/resources/device)
- [<span data-ttu-id="2f5ed-122">group</span><span class="sxs-lookup"><span data-stu-id="2f5ed-122">group</span></span>](/graph/api/resources/group)
- [<span data-ttu-id="2f5ed-123">servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="2f5ed-123">servicePrincipal</span></span>](/graph/api/resources/serviceprincipal)
- [<span data-ttu-id="2f5ed-124">user</span><span class="sxs-lookup"><span data-stu-id="2f5ed-124">user</span></span>](/graph/api/resources/user)

<span data-ttu-id="2f5ed-125">A tabela a seguir lista cenários de consulta em objetos de diretório que são suportados apenas em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-125">The following table lists query scenarios on directory objects that are supported only in advanced queries.</span></span>

| <span data-ttu-id="2f5ed-126">Descrição</span><span class="sxs-lookup"><span data-stu-id="2f5ed-126">Description</span></span>                                                              | <span data-ttu-id="2f5ed-127">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2f5ed-127">Example</span></span>                                                                                                                                                                                                                                                                                                                                                                                                                              |
|:-------------------------------------------------------------------------|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| <span data-ttu-id="2f5ed-128">Usar `$count` como um segmento URL</span><span class="sxs-lookup"><span data-stu-id="2f5ed-128">Use of `$count` as a URL segment</span></span>                                         | <span data-ttu-id="2f5ed-129">[GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-129">[GET](https://developer.microsoft.com/graph/graph-explorer?request=groups%2F%24count&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../groups/$count`</span></span>                                                                                                                                                                                       |
| <span data-ttu-id="2f5ed-130">Usar o `$count` como parâmetro consultar cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f5ed-130">Use of `$count` as a query string parameter</span></span>                              | <span data-ttu-id="2f5ed-131">[GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-131">[GET](https://developer.microsoft.com/graph/graph-explorer?request=servicePrincipals%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../servicePrincipals?$count=true`</span></span>                                                                                                                                                     |
| <span data-ttu-id="2f5ed-132">Usar de `$search`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-132">Use of `$search`</span></span>                                                         | <span data-ttu-id="2f5ed-133">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-133">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24search%3D%22displayName%3ABrowser%22&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$search="displayName:Browser"`</span></span>                                                                                                                     |
| <span data-ttu-id="2f5ed-134">Usar `$orderby` em propriedades selecionadas</span><span class="sxs-lookup"><span data-stu-id="2f5ed-134">Use of `$orderby` on select properties</span></span>                                   | <span data-ttu-id="2f5ed-135">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-135">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$count=true`</span></span>                                                                                                               |
| <span data-ttu-id="2f5ed-136">Usar o `$filter` com o `endsWith` operador</span><span class="sxs-lookup"><span data-stu-id="2f5ed-136">Use of `$filter` with the `endsWith` operator</span></span>                            | <span data-ttu-id="2f5ed-137">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-137">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24count%3Dtrue%26%24filter%3DendsWith(mail%2C'%40outlook.com')&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$count=true&$filter=endsWith(mail,'@outlook.com')`</span></span>                                                                                       |
| <span data-ttu-id="2f5ed-138">Usar o `$filter` e `$orderby` na mesma consulta</span><span class="sxs-lookup"><span data-stu-id="2f5ed-138">Use of `$filter` and `$orderby` in the same query</span></span>                        | <span data-ttu-id="2f5ed-139">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-139">[GET](https://developer.microsoft.com/graph/graph-explorer?request=applications%3F%24orderby%3DdisplayName%26%24filter%3DstartsWith(displayName%2C%20'Box')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../applications?$orderby=displayName&$filter=startsWith(displayName, 'Box')&$count=true`</span></span>                       |
| <span data-ttu-id="2f5ed-140">Uso o `$filter` com os `startsWith` operadores em propriedades específicas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-140">Use of `$filter` with the `startsWith` operators on specific properties.</span></span> | <span data-ttu-id="2f5ed-141">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-141">[GET](https://developer.microsoft.com/graph/graph-explorer?request=users%3F%24filter%3DstartsWith(mobilePhone%2C%20'25478')%20OR%20startsWith(mobilePhone%2C%20'25473')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=startsWith(mobilePhone, '25478') OR startsWith(mobilePhone, '25473')&$count=true`</span></span> |
| <span data-ttu-id="2f5ed-142">Usar o `$filter` com `ne` e `NOT` operadores</span><span class="sxs-lookup"><span data-stu-id="2f5ed-142">Use of `$filter` with `ne` and `NOT` operators</span></span>                           | <span data-ttu-id="2f5ed-143">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-143">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=users%3F%24filter%3DcompanyName%20ne%20null%20and%20NOT(companyName%20eq%20'Microsoft')%26%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=companyName ne null and NOT(companyName eq 'Microsoft')&$count=true`</span></span>                     |
| <span data-ttu-id="2f5ed-144">Usar o `$filter` com `NOT` e `startsWith` operadores</span><span class="sxs-lookup"><span data-stu-id="2f5ed-144">Use of `$filter` with `NOT` and `startsWith` operators</span></span>                   | <span data-ttu-id="2f5ed-145">
  [GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-145">[GET](https://developer.microsoft.com/en-us/graph/graph-explorer?request=%2Fusers%3F%24filter%3DNOT%20startsWith(displayName%2C%20'Conf')%26%24count%3Dtrue&method=GET&version=beta&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../users?$filter=NOT startsWith(displayName, 'Conf')&$count=true`</span></span>                                                                |
| <span data-ttu-id="2f5ed-146">Usar o molde de OData com outro parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="2f5ed-146">Use of OData cast with another query parameter</span></span>                           | <span data-ttu-id="2f5ed-147">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`</span><span class="sxs-lookup"><span data-stu-id="2f5ed-147">[GET](https://developer.microsoft.com/graph/graph-explorer?request=me%2FtransitiveMemberOf%2Fmicrosoft.graph.group%3F%24count%3Dtrue&method=GET&version=v1.0&GraphUrl=https://graph.microsoft.com&headers=W3sibmFtZSI6IkNvbnNpc3RlbmN5TGV2ZWwiLCJ2YWx1ZSI6ImV2ZW50dWFsIn1d) `../me/transitiveMemberOf/microsoft.graph.group?$count=true`</span></span>                                                                                             |

> [!NOTE]
> <span data-ttu-id="2f5ed-148">Estas capacidades avançadas de consulta não estão disponíveis nos locatários do Azure AD B2C.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-148">These advanced query capabilities are not available in Azure AD B2C tenants.</span></span>

## <a name="support-for-filter-on-properties-of-azure-ad-directory-objects"></a><span data-ttu-id="2f5ed-149">Suporte para filtro nas propriedades dos objetos do diretório Microsoft Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="2f5ed-149">Support for filter on properties of Azure AD directory objects</span></span>

<span data-ttu-id="2f5ed-150">As propriedades dos objetos de diretório se comportam de forma diferente em seu suporte aos parâmetros de consulta.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-150">Properties of directory objects behave differently in their support for query parameters.</span></span> <span data-ttu-id="2f5ed-151">Os cenários a seguir são comuns para objetos de diretório:</span><span class="sxs-lookup"><span data-stu-id="2f5ed-151">The following are common scenarios for directory objects:</span></span>

+ <span data-ttu-id="2f5ed-152">Salvo indicação em contrário, as propriedades com o mesmo nome nos recursos de diretório suportam os mesmos operadores `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-152">Unless otherwise indicated, properties with the same name across directory resources support the same `$filter` operators.</span></span> <span data-ttu-id="2f5ed-153">Por exemplo, a propriedade **createdDateTime** está disponível no **aplicação**, **grupo**, **organização**, e **usuário** recursos.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-153">For example, the **createdDateTime** property is available in **application**, **group**, **organization**, and **user** resources.</span></span> <span data-ttu-id="2f5ed-154">Ele suporta os operadores `eq`, `ge`, e `le` por padrão e os operadores `in`, `ne`, e `NOT` apenas em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-154">It supports the `eq`, `ge`, and `le` operators by default and the `in`, `ne`, and `NOT` operators only in advanced queries.</span></span>
+ <span data-ttu-id="2f5ed-155">O `endsWith` operador é suportado apenas em **email** e **userPrincipalNameerPrincipalName** propriedades.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-155">The `endsWith` operator is supported only on **mail** and **userPrincipalName** properties.</span></span>
+ <span data-ttu-id="2f5ed-156">Consultas que são suportadas por padrão também funcionarão em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-156">Queries that are supported by default will also work in advanced queries.</span></span>
+ <span data-ttu-id="2f5ed-157">Os operadores `NOT` e `ne` de negação são suportados apenas em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-157">The `NOT` and `ne` negation operators are supported only in advanced queries.</span></span> 
  + <span data-ttu-id="2f5ed-158">Todas as propriedades que suportam o `eq` operador também suportam os `ne` ou `NOT` operadores.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-158">All properties that support the `eq` operator also support the `ne` or `NOT` operators.</span></span>
  + <span data-ttu-id="2f5ed-159">O `ne` operador nega onde de outra forma o `eq` operador avaliaria para `true`.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-159">The `ne` operator negates where the `eq` operator would otherwise evaluate to `true`.</span></span> <span data-ttu-id="2f5ed-160">Para consultas que utilizam o `any` operador lambda, usar o `NOT` operador.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-160">For queries that use the `any` lambda operator, use the `NOT` operator.</span></span> <span data-ttu-id="2f5ed-161">Veja [Filtrar utilizando operadores lambda](/graph/query-parameters#filter-using-lambda-operators).</span><span class="sxs-lookup"><span data-stu-id="2f5ed-161">See [Filter using lambda operators](/graph/query-parameters#filter-using-lambda-operators).</span></span>

<span data-ttu-id="2f5ed-162">A tabela a seguir resume o suporte a `$filter` operadores por propriedades no [objeto de diretório](/graph/api/resources/user) de usuários.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-162">The following table summarizes support for `$filter` operators by properties on the [users](/graph/api/resources/user) directory object.</span></span>

- <span data-ttu-id="2f5ed-163">![Funciona por padrão.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-163">![Works by default.</span></span> <span data-ttu-id="2f5ed-164">Não requer parâmetros de consulta avançados.](/graph/images/advanced-query-parameters/default.png)</span><span class="sxs-lookup"><span data-stu-id="2f5ed-164">Does not require advanced query parameters.](/graph/images/advanced-query-parameters/default.png)</span></span> <span data-ttu-id="2f5ed-165">A propriedade suporta `$filter` com o operador por padrão.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-165">The property supports `$filter` with the operator by default.</span></span>
- <span data-ttu-id="2f5ed-166">![Requer parâmetros de consulta avançados.](/graph/images/advanced-query-parameters/advanced.png)</span><span class="sxs-lookup"><span data-stu-id="2f5ed-166">![Requires advanced query parameters.](/graph/images/advanced-query-parameters/advanced.png)</span></span> <span data-ttu-id="2f5ed-167">O operador específico `$filter` requer *parâmetros de consulta avançados*:</span><span class="sxs-lookup"><span data-stu-id="2f5ed-167">The specific `$filter` operator requires *advanced query parameters*:</span></span>
  - <span data-ttu-id="2f5ed-168">`ConsistencyLevel=eventual` cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2f5ed-168">`ConsistencyLevel=eventual` header</span></span>
  - <span data-ttu-id="2f5ed-169">`$count=true` cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2f5ed-169">`$count=true` query string</span></span>
- <span data-ttu-id="2f5ed-170">Células em branco indicam que a propriedade não suporta o uso de `$filter` com o operador.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-170">Blank cells indicate that the property does not support the use of `$filter` with the operator.</span></span>
- <span data-ttu-id="2f5ed-171">A coluna **valores nulos** indica que a propriedade é filtrável em `null` valores.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-171">The **null values** column indicates that the property is filterable on `null` values.</span></span>
- <span data-ttu-id="2f5ed-172">As propriedades que não estão listadas aqui não suportam `$filter`.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-172">Properties that are not listed here do not support `$filter`.</span></span>

[!INCLUDE [filter-directory-objects](../includes/filter-directory-objects.md)]


## <a name="error-handling-for-advanced-queries-on-directory-objects"></a><span data-ttu-id="2f5ed-173">Tratamento de erros para consultas avançadas sobre objetos de diretório</span><span class="sxs-lookup"><span data-stu-id="2f5ed-173">Error handling for advanced queries on directory objects</span></span>

<span data-ttu-id="2f5ed-174">A contagem de objetos de diretório só é suportada usando os parâmetros de consultas avançados.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-174">Counting directory objects is only supported using the advanced queries parameters.</span></span> <span data-ttu-id="2f5ed-175">Se o cabeçalho `ConsistencyLevel=eventual` não for especificado, o pedido retorna um erro quando o segmento `$count` URL é usado ou ignora silenciosamente o parâmetro `$count` consulta (`?$count=true`) se for usado.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-175">If the `ConsistencyLevel=eventual` header is not specified, the request returns an error when the `$count` URL segment is used or silently ignores the `$count` query parameter (`?$count=true`) if it's used.</span></span>

```http
https://graph.microsoft.com/v1.0/users/$count
```

```json
{
    "error": {
        "code": "Request_BadRequest",
        "message": "$count is not currently supported.",
        "innerError": {
            "date": "2021-05-18T19:03:10",
            "request-id": "d9bbd4d8-bb2d-44e6-99a1-71a9516da744",
            "client-request-id": "539da3bd-942f-25db-636b-27f6f6e8eae4"
        }
    }
}
```

<span data-ttu-id="2f5ed-176">`$search` nos recursos do Microsoft Azure Active Directory que derivam de [diretórioObject](/graph/api/resources/directoryobject) funciona apenas em consultas avançadas.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-176">`$search` on Azure AD resources that derive from [directoryObject](/graph/api/resources/directoryobject) works only in advanced queries.</span></span> <span data-ttu-id="2f5ed-177">Se o cabeçalho **ConsistencyLevel** não for especificado, o pedido retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-177">If the **ConsistencyLevel** header is not specified, the request returns an error.</span></span>

```http
https://graph.microsoft.com/v1.0/applications?$search="displayName:Browser"
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Request with $search query parameter only works through MSGraph with a special request header: 'ConsistencyLevel: eventual'",
        "innerError": {
            "date": "2021-05-27T14:26:47",
            "request-id": "9b600954-ba11-4899-8ce9-6abad341f299",
            "client-request-id": "7964ef27-13a3-6ca4-ed7b-73c271110867"
        }
    }
}
```

<span data-ttu-id="2f5ed-178">Se uma propriedade ou parâmetro de consulta na URL for suportado apenas em consultas avançadas, mas o cabeçalho **ConsistencyLevel** ou a cadeia de caracteres `$count=true` estiver faltando, a solicitação retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-178">If a property or query parameter in the URL is supported only in advanced queries but either the **ConsistencyLevel** header or the `$count=true` query string is missing, the request returns an error.</span></span>

```http
https://graph.microsoft.com/beta/users?$filter=endsWith(mail,'@outlook.com')
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "Unsupported Query.",
        "innerError": {
            "date": "2021-05-18T19:12:36",
            "request-id": "63f2093c-399c-4350-9609-3ce9b62abe3c",
            "client-request-id": "e60ed0ba-df5d-e190-f056-f9c0318456d7"
        }
    }
}
```

<span data-ttu-id="2f5ed-179">Se uma propriedade não tiver sido indexada para suportar um parâmetro de consulta, mesmo que os parâmetros de consulta avançados sejam especificados, a solicitação retorna um erro.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-179">If a property has not been indexed to support a query parameter, even if the advanced query parameters are specified, the request returns an error.</span></span>

```http
https://graph.microsoft.com/v1.0/users?$filter=id ge '398164b1-5196-49dd-ada2-364b49f99b27'&$count=true
ConsistencyLevel: eventual
```

```json
{
    "error": {
        "code": "Request_UnsupportedQuery",
        "message": "The request uses a filter property that is not indexed",
        "innerError": {
            "date": "2021-06-10T19:32:01",
            "request-id": "5625ba13-0c9f-4fce-a853-4b52f3e0bd09",
            "client-request-id": "76fe4cd8-df3a-f8c3-659b-594274b6bb31"
        }
    }
}
```

<span data-ttu-id="2f5ed-180">No entanto, é importante observar que os parâmetros de consulta especificados em uma solicitação podem falhar silenciosamente.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-180">However, it is important to note that query parameters specified in a request might fail silently.</span></span> <span data-ttu-id="2f5ed-181">Isso pode ser verdadeiro para parâmetros de consulta sem suporte, bem como para combinações de parâmetros de consulta sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-181">This can be true for unsupported query parameters as well as for unsupported combinations of query parameters.</span></span> <span data-ttu-id="2f5ed-182">Nesses casos, você deve examinar os dados retornados pela solicitação para determinar se os parâmetros de consulta que especificou tiveram o efeito desejado.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-182">In these cases, you should examine the data returned by the request to determine whether the query parameters you specified had the desired effect.</span></span> <span data-ttu-id="2f5ed-183">Por exemplo, no exemplo a seguir, falta o parâmetro `@odata.count` mesmo que a consulta seja bem sucedida.</span><span class="sxs-lookup"><span data-stu-id="2f5ed-183">For example, in the following example, the `@odata.count` parameter is missing even if the query is successful.</span></span>

```http
https://graph.microsoft.com/v1.0/users?$count=true
```

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "@odata.context":"https://graph.microsoft.com/v1.0/$metadata#users",
  "value":[
    {
      "displayName":"Oscar Ward",
      "mail":"oscarward@contoso.com",
      "userPrincipalName":"oscarward@contoso.com"
    },
  ]
}
```

## <a name="see-also"></a><span data-ttu-id="2f5ed-184">Confira também</span><span class="sxs-lookup"><span data-stu-id="2f5ed-184">See also</span></span>

- [<span data-ttu-id="2f5ed-185">Usar parâmetros de consulta para personalizar respostas</span><span class="sxs-lookup"><span data-stu-id="2f5ed-185">Use query parameters to customize responses</span></span>](/graph/query-parameters)
- [<span data-ttu-id="2f5ed-186">Limitações do parâmetro de consulta</span><span class="sxs-lookup"><span data-stu-id="2f5ed-186">Query parameter limitations</span></span>](known-issues.md#query-parameter-limitations)
- [<span data-ttu-id="2f5ed-187">Usar o parâmetro de consulta $search para corresponder a um critério de pesquisa</span><span class="sxs-lookup"><span data-stu-id="2f5ed-187">Use the $search query parameter to match a search criterion</span></span>](/graph/aad-advanced-queries)
