---
title: Adicionar dados personalizados aos usuários usando extensões abertas
description: 'Por meio de um exemplo, vamos demonstrar como usar o recurso *abrir extensões*. '
author: dkershaw10
ms.openlocfilehash: 37df1bd03e68b00be41496ee9f66a076d8758149
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27337167"
---
# <a name="add-custom-data-to-users-using-open-extensions"></a><span data-ttu-id="78483-103">Adicionar dados personalizados aos usuários usando extensões abertas</span><span class="sxs-lookup"><span data-stu-id="78483-103">Add custom data to users using open extensions</span></span>
<span data-ttu-id="78483-104">Por meio de um exemplo, vamos demonstrar como usar o recurso *abrir extensões*.</span><span class="sxs-lookup"><span data-stu-id="78483-104">We're going to walk you through an example to demonstrate how to use *open extensions*.</span></span> 

<span data-ttu-id="78483-p101">Imagine que você está criando um aplicativo que está disponível em várias plataformas cliente diferentes, como computadores e dispositivos móveis.  Você gostaria que os usuários pudessem configurar a própria experiência de interface do usuário para que ela fosse consistente, independentemente do dispositivo usado para entrar no seu aplicativo. Este é um requisito comum para a maioria dos aplicativos.</span><span class="sxs-lookup"><span data-stu-id="78483-p101">Imagine you're building an application that is available on lots of different client platforms, such as desktop and mobile.  You want to let users configure their UI experience so it’s consistent no matter which device they use to sign in to your app. This is a common requirement for most apps.</span></span> 

<span data-ttu-id="78483-108">Neste cenário, vamos mostrar como:</span><span class="sxs-lookup"><span data-stu-id="78483-108">For this scenario, we're going to show you how to:</span></span>

1. <span data-ttu-id="78483-109">Adicionar uma extensão aberta representando algumas informações do perfil móvel sobre o usuário.</span><span class="sxs-lookup"><span data-stu-id="78483-109">Add an open extension representing some roaming profile information about the user.</span></span>
2. <span data-ttu-id="78483-110">Consultar o usuário e retornar o perfil móvel.</span><span class="sxs-lookup"><span data-stu-id="78483-110">Query the user and return the roaming profile.</span></span>
3. <span data-ttu-id="78483-111">Alterar as informações do perfil móvel do usuário (o valor de extensão aberta).</span><span class="sxs-lookup"><span data-stu-id="78483-111">Change the user's roaming profile information (the open extension value).</span></span>
4. <span data-ttu-id="78483-112">Excluir informações do perfil móvel do usuário.</span><span class="sxs-lookup"><span data-stu-id="78483-112">Delete the user's roaming profile information.</span></span>

><span data-ttu-id="78483-p102">**Observação:** Este tópico mostra como adicionar, ler, atualizar e excluir extensões abertas em um recurso *user*.  Esses métodos também são suportados para os tipos de recurso *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* e *organizaton*.</span><span class="sxs-lookup"><span data-stu-id="78483-p102">**Note:** This topic shows you how to add, read, update and delete open extensions on a *user* resource.  These methods are also supported for the *administrativeUnit*, *contact*, *device*, *event*, *group*, *group event*, *group post* and *organizaton* resource types.</span></span>  
<span data-ttu-id="78483-p103">Basta atualizar as solicitações de exemplo abaixo usando qualquer um desses tipos de recursos. As respostas mostradas nos exemplos a seguir podem ser truncadas para resumir.</span><span class="sxs-lookup"><span data-stu-id="78483-p103">Simply update the example requests below using any of those resource types. The responses shown in the examples below may be truncated for brevity.</span></span> 

## <a name="1-add-roaming-profile-information"></a><span data-ttu-id="78483-117">1. Adicionar informações de perfil móvel</span><span class="sxs-lookup"><span data-stu-id="78483-117">1. Add roaming profile information</span></span>
<span data-ttu-id="78483-p104">O usuário entra no aplicativo e configura a aparência do aplicativo.  Essas configurações de aplicativo devem transitar para que o usuário obtenha a mesma experiência em praticamente qualquer dispositivo usado para entrar no aplicativo.  Aqui, veremos como adicionar as informações do perfil móvel a um recurso user.</span><span class="sxs-lookup"><span data-stu-id="78483-p104">The user signs in to the app and configures the look and feel of the app.  These app settings should roam so that the user gets the same experience on whatever device they sign in to the app from.  Here we'll see how to add the roaming profile information to a user resource.</span></span>

##### <a name="request"></a><span data-ttu-id="78483-121">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78483-121">Request</span></span>
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
##### <a name="response"></a><span data-ttu-id="78483-122">Resposta</span><span class="sxs-lookup"><span data-stu-id="78483-122">Response</span></span>
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

## <a name="2-retrieve-roaming-profile-information"></a><span data-ttu-id="78483-123">2. Recuperar informações do perfil móvel do usuário.</span><span class="sxs-lookup"><span data-stu-id="78483-123">2. Retrieve roaming profile information</span></span>
<span data-ttu-id="78483-p105">Quando o usuário entra no aplicativo de outro dispositivo, o aplicativo pode recuperar detalhes do perfil do usuário, além das configurações de roaming dele. Isso pode ser feito obtendo recursos do usuário e expandindo a propriedade de navegação da extensão.</span><span class="sxs-lookup"><span data-stu-id="78483-p105">When the user signs in to the app from another device, the app can retrieve the user's profile details as well as their roaming settings. This can be done by getting the user's resource and expanding the extension navigation property.</span></span>

##### <a name="request"></a><span data-ttu-id="78483-126">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78483-126">Request</span></span>
```http
GET https://graph.microsoft.com/v1.0/me?$select=id,displayName,mail,mobilePhone&$expand=extensions
```
##### <a name="response"></a><span data-ttu-id="78483-127">Resposta</span><span class="sxs-lookup"><span data-stu-id="78483-127">Response</span></span>
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
><span data-ttu-id="78483-128">**Observação:** Se você tiver várias extensões, filtre o *id* para obter a extensão na qual está interessado.</span><span class="sxs-lookup"><span data-stu-id="78483-128">**Note:** If you have multiple extensions, you can filter on the *id* to get the extension that you are interested in.</span></span>

## <a name="3-change-roaming-profile-information"></a><span data-ttu-id="78483-129">3. Alterar informações de perfil móvel</span><span class="sxs-lookup"><span data-stu-id="78483-129">3. Change roaming profile information</span></span>
<span data-ttu-id="78483-p106">O usuário pode optar por alterar as próprias informações do perfil móvel.  Essa atualização pode ser feita com um ```PATCH``` no valor da extensão aberta.</span><span class="sxs-lookup"><span data-stu-id="78483-p106">The user may choose to change their roaming profile information.  This update can be done with a ```PATCH``` on the open extension value.</span></span> 

##### <a name="request"></a><span data-ttu-id="78483-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78483-132">Request</span></span>
```http
PATCH https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
Content-type: application/json
{
    "theme":"light",
    "color":"yellow",
    "lang":"Swahili"
}
```

##### <a name="response"></a><span data-ttu-id="78483-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="78483-133">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="4-delete-a-users-roaming-profile"></a><span data-ttu-id="78483-134">4. Excluir um perfil de usuário móvel</span><span class="sxs-lookup"><span data-stu-id="78483-134">4. Delete a user's roaming profile</span></span>
<span data-ttu-id="78483-p107">O usuário decide que, se não quiser mais um perfil móvel, pode excluí-lo. Esta atualização pode ser feita com uma solicitação ```DELETE``` no valor extensão aberto.</span><span class="sxs-lookup"><span data-stu-id="78483-p107">The user decides that they don't want a roaming profile anymore, so they delete it. This can be done with a ```DELETE``` request on the open extension value.</span></span>

##### <a name="request"></a><span data-ttu-id="78483-137">Solicitação</span><span class="sxs-lookup"><span data-stu-id="78483-137">Request</span></span>
```http
DELETE https://graph.microsoft.com/v1.0/me/extensions/com.contoso.roamingSettings
```

##### <a name="response"></a><span data-ttu-id="78483-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="78483-138">Response</span></span>
```
HTTP/1.1 204 No content
```

## <a name="see-also"></a><span data-ttu-id="78483-139">Confira também</span><span class="sxs-lookup"><span data-stu-id="78483-139">See also</span></span>

- [<span data-ttu-id="78483-140">Adicionar dados personalizados a recursos usando extensões</span><span class="sxs-lookup"><span data-stu-id="78483-140">Add custom data to resources using extensions</span></span>](extensibility-overview.md)
- [<span data-ttu-id="78483-141">Adicionar dados personalizados a grupos usando as extensões do esquema</span><span class="sxs-lookup"><span data-stu-id="78483-141">Add custom data to groups using schema extensions</span></span>](extensibility-schema-groups.md)
- [<span data-ttu-id="78483-142">tipo de recurso openTypeExtension</span><span class="sxs-lookup"><span data-stu-id="78483-142">openTypeExtension resource type</span></span>](/graph/api/resources/opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="78483-143">Criar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="78483-143">Create open extension</span></span>](/graph/api/opentypeextension-post-opentypeextension?view=graph-rest-1.0)
- [<span data-ttu-id="78483-144">Obter extensão aberta</span><span class="sxs-lookup"><span data-stu-id="78483-144">Get open extension</span></span>](/graph/api/opentypeextension-get?view=graph-rest-1.0)
- [<span data-ttu-id="78483-145">Atualizar extensão aberta</span><span class="sxs-lookup"><span data-stu-id="78483-145">Update open extension</span></span>](/graph/api/opentypeextension-update?view=graph-rest-1.0)
- [<span data-ttu-id="78483-146">Excluir extensão aberta</span><span class="sxs-lookup"><span data-stu-id="78483-146">Delete open extension</span></span>](/graph/api/opentypeextension-delete?view=graph-rest-1.0)