---
title: Tipo de recurso windowsHelloForBusinessAuthenticationMethod
description: Uma representação de uma instância do Windows Hello para Empresas registrada para um usuário. O Windows Hello para Empresas é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: dcbbebf03a91563e5504eb3032f57f973a4c3ede
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/26/2021
ms.locfileid: "49982478"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a><span data-ttu-id="a0517-104">Tipo de recurso windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0517-104">windowsHelloForBusinessAuthenticationMethod resource type</span></span>

<span data-ttu-id="a0517-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a0517-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a0517-106">Uma representação de um método de autenticação do Windows Hello para Empresas registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="a0517-106">A representation of a Windows Hello for Business authentication method registered to a user.</span></span> <span data-ttu-id="a0517-107">O Windows Hello para Empresas é um método de autenticação de entrada para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="a0517-107">Windows Hello for Business is a sign-in authentication method for Windows devices.</span></span>

<span data-ttu-id="a0517-108">Herda de [authenticationMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="a0517-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="a0517-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="a0517-109">Methods</span></span>
|<span data-ttu-id="a0517-110">Método</span><span class="sxs-lookup"><span data-stu-id="a0517-110">Method</span></span>|<span data-ttu-id="a0517-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a0517-111">Return type</span></span>|<span data-ttu-id="a0517-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0517-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="a0517-113">Listar windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="a0517-113">List windowsHelloForBusinessAuthenticationMethods</span></span>](../api/windowshelloforbusinessauthenticationmethod-list.md)|<span data-ttu-id="a0517-114">[Coleção windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a0517-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) collection</span></span>|<span data-ttu-id="a0517-115">Obter uma lista dos [objetos windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="a0517-115">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="a0517-116">Obter windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0517-116">Get windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-get.md)|[<span data-ttu-id="a0517-117">windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0517-117">windowsHelloForBusinessAuthenticationMethod</span></span>](../resources/windowshelloforbusinessauthenticationmethod.md)|<span data-ttu-id="a0517-118">Leia as propriedades e as relações de um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a0517-118">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="a0517-119">Excluir windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0517-119">Delete windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-delete.md)|<span data-ttu-id="a0517-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0517-120">None</span></span>|<span data-ttu-id="a0517-121">Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a0517-121">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="a0517-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0517-122">Properties</span></span>
|<span data-ttu-id="a0517-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0517-123">Property</span></span>|<span data-ttu-id="a0517-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0517-124">Type</span></span>|<span data-ttu-id="a0517-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0517-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0517-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a0517-126">createdDateTime</span></span>|<span data-ttu-id="a0517-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0517-127">DateTimeOffset</span></span>|<span data-ttu-id="a0517-128">A data e a hora em que essa chave do Windows Hello para Empresas foi registrada.</span><span class="sxs-lookup"><span data-stu-id="a0517-128">The date and time that this Windows Hello for Business key was registered.</span></span>|
|<span data-ttu-id="a0517-129">displayName</span><span class="sxs-lookup"><span data-stu-id="a0517-129">displayName</span></span>|<span data-ttu-id="a0517-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0517-130">String</span></span>|<span data-ttu-id="a0517-131">O nome do dispositivo no qual o Windows Hello para Empresas está registrado</span><span class="sxs-lookup"><span data-stu-id="a0517-131">The name of the device on which Windows Hello for Business is registered</span></span>|
|<span data-ttu-id="a0517-132">id</span><span class="sxs-lookup"><span data-stu-id="a0517-132">id</span></span>|<span data-ttu-id="a0517-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0517-133">String</span></span>|<span data-ttu-id="a0517-134">Um identificador exclusivo para esse método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="a0517-134">A unique identifier for this authentication method.</span></span> <span data-ttu-id="a0517-135">Herdado de [authenticationMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="a0517-135">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="a0517-136">keyStrength</span><span class="sxs-lookup"><span data-stu-id="a0517-136">keyStrength</span></span>|<span data-ttu-id="a0517-137">authenticationMethodKeyStrength</span><span class="sxs-lookup"><span data-stu-id="a0517-137">authenticationMethodKeyStrength</span></span>|<span data-ttu-id="a0517-138">Força fundamental dessa chave do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="a0517-138">Key strength of this Windows Hello for Business key.</span></span> <span data-ttu-id="a0517-139">Os valores possíveis são: `normal`, `weak`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="a0517-139">Possible values are: `normal`, `weak`, `unknown`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0517-140">Relações</span><span class="sxs-lookup"><span data-stu-id="a0517-140">Relationships</span></span>
|<span data-ttu-id="a0517-141">Relação</span><span class="sxs-lookup"><span data-stu-id="a0517-141">Relationship</span></span>|<span data-ttu-id="a0517-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0517-142">Type</span></span>|<span data-ttu-id="a0517-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0517-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0517-144">device</span><span class="sxs-lookup"><span data-stu-id="a0517-144">device</span></span>|[<span data-ttu-id="a0517-145">device</span><span class="sxs-lookup"><span data-stu-id="a0517-145">device</span></span>](../resources/device.md)|<span data-ttu-id="a0517-146">O dispositivo registrado no qual esta chave do Windows Hello para Empresas reside.</span><span class="sxs-lookup"><span data-stu-id="a0517-146">The registered device on which this Windows Hello for Business key resides.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a0517-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0517-147">JSON representation</span></span>
<span data-ttu-id="a0517-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0517-148">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsHelloForBusinessAuthenticationMethod",
  "id": "String (Identifier)",
  "displayName": "String",
  "createdDateTime": "String",
  "keyStrength": {"@odata.type": "microsoft.graph.authenticationMethodKeyStrength"}
}
```
