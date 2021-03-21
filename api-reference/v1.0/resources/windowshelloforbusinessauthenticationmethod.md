---
title: Tipo de recurso windowsHelloForBusinessAuthenticationMethod
description: Uma representação de uma instância do Windows Hello para Empresas registrada em um usuário. O Windows Hello para Empresas é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ad3fd83605d49351e2c57b469339fcfe222f05cb
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50964585"
---
# <a name="windowshelloforbusinessauthenticationmethod-resource-type"></a><span data-ttu-id="f599e-104">Tipo de recurso windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f599e-104">windowsHelloForBusinessAuthenticationMethod resource type</span></span>

<span data-ttu-id="f599e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f599e-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="f599e-106">Uma representação de um método de autenticação do Windows Hello para Empresas registrado para um usuário.</span><span class="sxs-lookup"><span data-stu-id="f599e-106">A representation of a Windows Hello for Business authentication method registered to a user.</span></span> <span data-ttu-id="f599e-107">O Windows Hello para Empresas é um método de autenticação de entrada para dispositivos Windows.</span><span class="sxs-lookup"><span data-stu-id="f599e-107">Windows Hello for Business is a sign-in authentication method for Windows devices.</span></span>

<span data-ttu-id="f599e-108">Herda de [authenticationMethod](../resources/authenticationmethod.md).</span><span class="sxs-lookup"><span data-stu-id="f599e-108">Inherits from [authenticationMethod](../resources/authenticationmethod.md).</span></span>

## <a name="methods"></a><span data-ttu-id="f599e-109">Métodos</span><span class="sxs-lookup"><span data-stu-id="f599e-109">Methods</span></span>
|<span data-ttu-id="f599e-110">Método</span><span class="sxs-lookup"><span data-stu-id="f599e-110">Method</span></span>|<span data-ttu-id="f599e-111">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="f599e-111">Return type</span></span>|<span data-ttu-id="f599e-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="f599e-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="f599e-113">Listar windowsHelloForBusinessAuthenticationMethods</span><span class="sxs-lookup"><span data-stu-id="f599e-113">List windowsHelloForBusinessAuthenticationMethods</span></span>](../api/windowshelloforbusinessauthenticationmethod-list.md)|<span data-ttu-id="f599e-114">[coleção windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f599e-114">[windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) collection</span></span>|<span data-ttu-id="f599e-115">Obter uma lista dos [objetos windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="f599e-115">Get a list of the [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) objects and their properties.</span></span>|
|[<span data-ttu-id="f599e-116">Obter windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f599e-116">Get windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-get.md)|[<span data-ttu-id="f599e-117">windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f599e-117">windowsHelloForBusinessAuthenticationMethod</span></span>](../resources/windowshelloforbusinessauthenticationmethod.md)|<span data-ttu-id="f599e-118">Leia as propriedades e as relações de um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f599e-118">Read the properties and relationships of a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|
|[<span data-ttu-id="f599e-119">Excluir windowsHelloForBusinessAuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="f599e-119">Delete windowsHelloForBusinessAuthenticationMethod</span></span>](../api/windowshelloforbusinessauthenticationmethod-delete.md)|<span data-ttu-id="f599e-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f599e-120">None</span></span>|<span data-ttu-id="f599e-121">Exclui um [objeto windowsHelloForBusinessAuthenticationMethod.](../resources/windowshelloforbusinessauthenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f599e-121">Deletes a [windowsHelloForBusinessAuthenticationMethod](../resources/windowshelloforbusinessauthenticationmethod.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="f599e-122">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f599e-122">Properties</span></span>
|<span data-ttu-id="f599e-123">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f599e-123">Property</span></span>|<span data-ttu-id="f599e-124">Tipo</span><span class="sxs-lookup"><span data-stu-id="f599e-124">Type</span></span>|<span data-ttu-id="f599e-125">Descrição</span><span class="sxs-lookup"><span data-stu-id="f599e-125">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f599e-126">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f599e-126">createdDateTime</span></span>|<span data-ttu-id="f599e-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f599e-127">DateTimeOffset</span></span>|<span data-ttu-id="f599e-128">A data e a hora em que essa chave do Windows Hello para Empresas foi registrada.</span><span class="sxs-lookup"><span data-stu-id="f599e-128">The date and time that this Windows Hello for Business key was registered.</span></span>|
|<span data-ttu-id="f599e-129">displayName</span><span class="sxs-lookup"><span data-stu-id="f599e-129">displayName</span></span>|<span data-ttu-id="f599e-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f599e-130">String</span></span>|<span data-ttu-id="f599e-131">O nome do dispositivo no qual o Windows Hello para Empresas está registrado</span><span class="sxs-lookup"><span data-stu-id="f599e-131">The name of the device on which Windows Hello for Business is registered</span></span>|
|<span data-ttu-id="f599e-132">id</span><span class="sxs-lookup"><span data-stu-id="f599e-132">id</span></span>|<span data-ttu-id="f599e-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f599e-133">String</span></span>|<span data-ttu-id="f599e-134">Um identificador exclusivo para esse método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="f599e-134">A unique identifier for this authentication method.</span></span> <span data-ttu-id="f599e-135">Herdado da [autenticaçãoMethod](../resources/authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="f599e-135">Inherited from [authenticationMethod](../resources/authenticationmethod.md)</span></span>|
|<span data-ttu-id="f599e-136">keyStrength</span><span class="sxs-lookup"><span data-stu-id="f599e-136">keyStrength</span></span>|<span data-ttu-id="f599e-137">authenticationMethodKeyStrength</span><span class="sxs-lookup"><span data-stu-id="f599e-137">authenticationMethodKeyStrength</span></span>|<span data-ttu-id="f599e-138">Força fundamental dessa chave do Windows Hello para Empresas.</span><span class="sxs-lookup"><span data-stu-id="f599e-138">Key strength of this Windows Hello for Business key.</span></span> <span data-ttu-id="f599e-139">Os valores possíveis são: `normal`, `weak`, `unknown`.</span><span class="sxs-lookup"><span data-stu-id="f599e-139">Possible values are: `normal`, `weak`, `unknown`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f599e-140">Relações</span><span class="sxs-lookup"><span data-stu-id="f599e-140">Relationships</span></span>
|<span data-ttu-id="f599e-141">Relação</span><span class="sxs-lookup"><span data-stu-id="f599e-141">Relationship</span></span>|<span data-ttu-id="f599e-142">Tipo</span><span class="sxs-lookup"><span data-stu-id="f599e-142">Type</span></span>|<span data-ttu-id="f599e-143">Descrição</span><span class="sxs-lookup"><span data-stu-id="f599e-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f599e-144">device</span><span class="sxs-lookup"><span data-stu-id="f599e-144">device</span></span>|[<span data-ttu-id="f599e-145">device</span><span class="sxs-lookup"><span data-stu-id="f599e-145">device</span></span>](../resources/device.md)|<span data-ttu-id="f599e-146">O dispositivo registrado no qual esta chave do Windows Hello para Empresas reside.</span><span class="sxs-lookup"><span data-stu-id="f599e-146">The registered device on which this Windows Hello for Business key resides.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f599e-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f599e-147">JSON representation</span></span>
<span data-ttu-id="f599e-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f599e-148">The following is a JSON representation of the resource.</span></span>
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
