---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 11c0598f19fcc5bf6f9862a2d87fa1f08acb8a2c
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/20/2021
ms.locfileid: "50945666"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="5235e-104">Tipo de recurso fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5235e-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="5235e-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5235e-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5235e-106">Uma representação de uma chave de segurança FIDO2 registrada em um usuário.</span><span class="sxs-lookup"><span data-stu-id="5235e-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="5235e-107">FIDO2 é um método de autenticação de login.</span><span class="sxs-lookup"><span data-stu-id="5235e-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="5235e-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="5235e-108">Methods</span></span>
|<span data-ttu-id="5235e-109">Método</span><span class="sxs-lookup"><span data-stu-id="5235e-109">Method</span></span>|<span data-ttu-id="5235e-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="5235e-110">Return type</span></span>|<span data-ttu-id="5235e-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5235e-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5235e-112">List</span><span class="sxs-lookup"><span data-stu-id="5235e-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="5235e-113">[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="5235e-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="5235e-114">Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="5235e-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="5235e-115">Get</span><span class="sxs-lookup"><span data-stu-id="5235e-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="5235e-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="5235e-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="5235e-117">Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5235e-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="5235e-118">Delete</span><span class="sxs-lookup"><span data-stu-id="5235e-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="5235e-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5235e-119">None</span></span>|<span data-ttu-id="5235e-120">Exclui o objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="5235e-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5235e-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5235e-121">Properties</span></span>
|<span data-ttu-id="5235e-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5235e-122">Property</span></span>|<span data-ttu-id="5235e-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="5235e-123">Type</span></span>|<span data-ttu-id="5235e-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="5235e-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5235e-125">id</span><span class="sxs-lookup"><span data-stu-id="5235e-125">id</span></span>|<span data-ttu-id="5235e-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5235e-126">String</span></span>|<span data-ttu-id="5235e-127">O identificador do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="5235e-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="5235e-128">displayName</span><span class="sxs-lookup"><span data-stu-id="5235e-128">displayName</span></span>|<span data-ttu-id="5235e-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5235e-129">String</span></span>|<span data-ttu-id="5235e-130">O nome de exibição da chave conforme dado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="5235e-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="5235e-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="5235e-131">creationDateTime</span></span>|<span data-ttu-id="5235e-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5235e-132">DateTimeOffset</span></span>|<span data-ttu-id="5235e-133">O timestamp quando essa chave foi registrada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="5235e-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="5235e-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="5235e-134">aaGuid</span></span>|<span data-ttu-id="5235e-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="5235e-135">String</span></span>|<span data-ttu-id="5235e-136">GUID de Atestado de Autenticador, um identificador que indica o tipo (por exemplo, make e model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="5235e-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="5235e-137">modelo</span><span class="sxs-lookup"><span data-stu-id="5235e-137">model</span></span>|<span data-ttu-id="5235e-138">String</span><span class="sxs-lookup"><span data-stu-id="5235e-138">String</span></span>|<span data-ttu-id="5235e-139">O modelo atribuído pelo fabricante da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="5235e-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="5235e-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="5235e-140">attestationCertificates</span></span>|<span data-ttu-id="5235e-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="5235e-141">String collection</span></span>|<span data-ttu-id="5235e-142">Os certificados de atestado anexados a essa chave de segurança.</span><span class="sxs-lookup"><span data-stu-id="5235e-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="5235e-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="5235e-143">attestationLevel</span></span>|<span data-ttu-id="5235e-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="5235e-144">attestationLevel</span></span>|<span data-ttu-id="5235e-145">O nível de atestado dessa chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="5235e-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="5235e-146">Os valores possíveis são: `attested`, `notAttested`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="5235e-146">Possible values are: `attested`, `notAttested`, `unknownFutureValue`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="5235e-147">Relações</span><span class="sxs-lookup"><span data-stu-id="5235e-147">Relationships</span></span>
<span data-ttu-id="5235e-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5235e-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="5235e-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5235e-149">JSON representation</span></span>
<span data-ttu-id="5235e-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5235e-150">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.fido2AuthenticationMethod",
  "baseType": "microsoft.graph.authenticationMethod",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.fido2AuthenticationMethod",
  "id": "String (identifier)",
  "displayName": "String",
  "creationDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

