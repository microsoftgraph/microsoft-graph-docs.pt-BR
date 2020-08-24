---
title: Adicionar dados personalizados aos usuários usando extensões abertas
description: 'Neste artigo você será guiado através de um exemplo para ilustrar o uso de *extensões abertas*. '
author: dkershaw10
localization_priority: Priority
ms.custom: graphiamtop20
ms.openlocfilehash: 81c1d77ecc2e57dec9ae18bf298d7390b71651dc
ms.sourcegitcommit: 1f8dc8750a50fb624a33e1d6360d29af38fa9514
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/21/2020
ms.locfileid: "46849090"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a><span data-ttu-id="e0c99-103">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="e0c99-103">Add custom data to users using open extensions</span></span>
<span data-ttu-id="e0c99-104">Neste artigo você será guiado através de um exemplo para ilustrar o uso de *extensões abertas*.</span><span class="sxs-lookup"><span data-stu-id="e0c99-104">This article walks you through an example to demonstrate how to use *open extensions*.</span></span> 

<span data-ttu-id="e0c99-p101">Imagine que você está criando um aplicativo que está disponível em várias plataformas cliente diferentes, como computadores e dispositivos móveis.  Você gostaria que os usuários pudessem configurar a própria experiência de interface do usuário para que ela fosse consistente, independentemente do dispositivo usado para entrar no seu aplicativo. Este é um requisito comum para a maioria dos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="e0c99-p101">Imagine you're building an application that is available on lots of different client platforms, such as desktop and mobile.  You want to let users configure their UI experience so it’s consistent no matter which device they use to sign in to your app. This is a common requirement for most apps.</span></span> 

<span data-ttu-id="e0c99-108">Para este cenário, este artigo lhe mostrará como:</span><span class="sxs-lookup"><span data-stu-id="e0c99-108">For this scenario, this article will show you how to:</span></span>

1. <span data-ttu-id="e0c99-109">Adicionar uma extensão aberta representando algumas informações do perfil móvel sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="e0c99-109">Add an open extension representing some roaming profile information about the user.</span></span>
2. <span data-ttu-id="e0c99-110">Consultar o usuário e retornar o perfil móvel.</span><span class="sxs-lookup"><span data-stu-id="e0c99-110">Query the user and return the roaming profile.</span></span>
3. <span data-ttu-id="e0c99-111">Alterar as informações do perfil móvel do usuário (o valor de extensão aberta).</span><span class="sxs-lookup"><span data-stu-id="e0c99-111">Change the user's roaming profile information (the open extension value).</span></span>
4. <span data-ttu-id="e0c99-112">Excluir informações do perfil móvel do usuário.</span><span class="sxs-lookup"><span data-stu-id="e0c99-112">Delete the user's roaming profile information.</span></span>

><span data-ttu-id="e0c99-p102">**Observação:** Este tópico mostrará a você como adicionar, ler, atualizar e excluir extensões abertas em um recurso de **user**. Esses métodos também são suportados para os tipos de recurso **administrativeUnit**, **contact**, **device**, **event**, **group**, **organization**, **post**, **todoTask**, e **todoTaskList**.</span><span class="sxs-lookup"><span data-stu-id="e0c99-p102">**Note:** This topic shows you how to add, read, update and delete open extensions on a **user** resource. These methods are also supported for the **administrativeUnit**, **contact**, **device**, **event**, **group**, **organizaton**, **post**, **todoTask**, and **todoTaskList** resource types.</span></span>  
<span data-ttu-id="e0c99-115">Você pode atualizar os exemplos de solicitação usando qualquer um desses tipos de recursos.</span><span class="sxs-lookup"><span data-stu-id="e0c99-115">You can update the request examples using any of those resource types.</span></span> <span data-ttu-id="e0c99-116">As respostas ilustradas nos exemplos poderiam ser reduzidas para facilitar a leitura.</span><span class="sxs-lookup"><span data-stu-id="e0c99-116">The responses shown in the examples might be shortened for readability.</span></span> 

## <a name="1-add-roaming-profile-information"></a><span data-ttu-id="e0c99-117">1. Adicionar informações de perfil móvel</span><span class="sxs-lookup"><span data-stu-id="e0c99-117">1. Add roaming profile information</span></span>
<span data-ttu-id="e0c99-p104">O usuário entra no aplicativo e configura a aparência do aplicativo.  Essas configurações de aplicativo devem transitar para que o usuário obtenha a mesma experiência em praticamente qualquer dispositivo usado para entrar no aplicativo.  Aqui, veremos como adicionar as informações do perfil móvel a um recurso user.</span><span class="sxs-lookup"><span data-stu-id="e0c99-p104">The user signs in to the app and configures the look and feel of the app.  These app settings should roam so that the user gets the same experience on whatever device they sign in to the app from.  Here we'll see how to add the roaming profile information to a user resource.</span></span>

### <a name="request"></a><span data-ttu-id="e0c99-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c99-121">Request</span></span>
```http
POST https://graph.microsoft.com/v1.0/me/extensions
Content-type: application/json
{
    "@odata.type":"microsoft.graph.openTypeExtension",
    "extensionName":"com.contoso.roamingSettings",
    "theme":"dark",
    "color":"purple",
    "lang":"Japanese"
}
```
### <a name="response"></a><span data-ttu-id="e0c99-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c99-122">Response</span></span>
```http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 420

{
    "@odata.type": "#microsoft.graph.openTypeExtension",
    "extensionName": "com.contoso.roamingSettings",
    "id": "com.contoso.roamingSettings",
    "theme": "dark",
    "color": "purple",
    "lang": "Japanese"
}
```

## <a name="2-retrieve-roaming-profile-information"></a><span data-ttu-id="e0c99-123">2. Recuperar informações do perfil móvel do usuário.</span><span class="sxs-lookup"><span data-stu-id="e0c99-123">2. Retrieve roaming profile information</span></span>
<span data-ttu-id="e0c99-p105">Quando o usuário entra no aplicativo de outro dispositivo, o aplicativo pode recuperar detalhes do perfil do usuário, além das configurações de roaming dele. Isso pode ser feito obtendo recursos do usuário e expandindo a propriedade de navegação da extensão.</span><span class="sxs-lookup"><span data-stu-id="e0c99-p105">When the user signs in to the app from another device, the app can retrieve the user's profile details as well as their roaming settings. This can be done by getting the user's resource and expanding the extension navigation property.</span></span>

### <a name="request"></a><span data-ttu-id="e0c99-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c99-126">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
### <a name="response"></a><span data-ttu-id="e0c99-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c99-127">Response</span></span>
```http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 420

{
    "id": "84b80893-8749-40a3-97b7-68513b600544",
    "displayName": "John Smith",
    "mail": "john@contoso.com",
    "mobilePhone": "1-555-6589",
    "extensions": [
        {
            "@odata.type": "#microsoft.graph.openTypeExtension",
            "extensionName": "com.contoso.roamingSettings",
            "id": "com.contoso.roamingSettings",
            "theme": "dark",
            "color": "purple",
            "lang": "Japanese"
        }
    ]
}
```
><span data-ttu-id="e0c99-128">**Observação:** Se você tiver várias extensões, você pode filtrar na **id** para obter a extensão que lhe interessa.</span><span class="sxs-lookup"><span data-stu-id="e0c99-128">**Note:** If you have multiple extensions, you can filter on the **id** to get the extension that you're interested in.</span></span>

## <a name="3-change-roaming-profile-information"></a><span data-ttu-id="e0c99-129">3. Alterar informações de perfil móvel</span><span class="sxs-lookup"><span data-stu-id="e0c99-129">3. Change roaming profile information</span></span>
<span data-ttu-id="e0c99-p106">O usuário pode escolher alterar as próprias informações do perfil móvel.  Esta atualização pode ser feita com um ```PATCH``` no valor da extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="e0c99-p106">The user can choose to change their roaming profile information.  This update can be done with a ```PATCH``` on the open extension value.</span></span> 

### <a name="request"></a><span data-ttu-id="e0c99-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c99-132">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

### <a name="response"></a><span data-ttu-id="e0c99-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c99-133">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a><span data-ttu-id="e0c99-134">4. Excluir um perfil de usuário móvel</span><span class="sxs-lookup"><span data-stu-id="e0c99-134">4. Delete a user's roaming profile</span></span>
<span data-ttu-id="e0c99-p107">O usuário decide que, se não quiser mais um perfil móvel, pode excluí-lo. Esta atualização pode ser feita com uma solicitação ```DELETE``` no valor extensão aberto.</span><span class="sxs-lookup"><span data-stu-id="e0c99-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>

### <a name="request"></a><span data-ttu-id="e0c99-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e0c99-137">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

### <a name="response"></a><span data-ttu-id="e0c99-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="e0c99-138">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="e0c99-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="e0c99-139">See also</span></span>

- [<span data-ttu-id="e0c99-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="e0c99-140">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="e0c99-141">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="e0c99-141">Add custom data to groups using schema extensions</span></span>](extensibility-schema-groups.md)
- [<span data-ttu-id="e0c99-142">tipo de recurso openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="e0c99-142">openTypeExtension resource type</span></span>](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="e0c99-143">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="e0c99-143">Create open extension</span></span>](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="e0c99-144">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="e0c99-144">Get open extension</span></span>](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="e0c99-145">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="e0c99-145">Update open extension</span></span>](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="e0c99-146">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="e0c99-146">Delete open extension</span></span>](/graph/api/opentypeextension-delete?view=graph-rest-1.0)
