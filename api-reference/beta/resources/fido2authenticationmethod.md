---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: a6cfed32f6e657608b70c799d348c6818e56a8c7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50440322"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="8a1fc-104">Tipo de recurso fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8a1fc-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="8a1fc-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8a1fc-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8a1fc-106">Uma representação de uma chave de segurança FIDO2 registrada em um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="8a1fc-107">FIDO2 é um método de autenticação de login.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="8a1fc-108">Methods</span><span class="sxs-lookup"><span data-stu-id="8a1fc-108">Methods</span></span>
|<span data-ttu-id="8a1fc-109">Método</span><span class="sxs-lookup"><span data-stu-id="8a1fc-109">Method</span></span>|<span data-ttu-id="8a1fc-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="8a1fc-110">Return type</span></span>|<span data-ttu-id="8a1fc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a1fc-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="8a1fc-112">List</span><span class="sxs-lookup"><span data-stu-id="8a1fc-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="8a1fc-113">[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="8a1fc-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="8a1fc-114">Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="8a1fc-115">Get</span><span class="sxs-lookup"><span data-stu-id="8a1fc-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="8a1fc-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8a1fc-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="8a1fc-117">Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="8a1fc-118">Delete</span><span class="sxs-lookup"><span data-stu-id="8a1fc-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="8a1fc-119">Nenhum(a)</span><span class="sxs-lookup"><span data-stu-id="8a1fc-119">None</span></span>|<span data-ttu-id="8a1fc-120">Exclui o objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="8a1fc-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8a1fc-121">Properties</span></span>
|<span data-ttu-id="8a1fc-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8a1fc-122">Property</span></span>|<span data-ttu-id="8a1fc-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="8a1fc-123">Type</span></span>|<span data-ttu-id="8a1fc-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="8a1fc-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8a1fc-125">id</span><span class="sxs-lookup"><span data-stu-id="8a1fc-125">id</span></span>|<span data-ttu-id="8a1fc-126">String</span><span class="sxs-lookup"><span data-stu-id="8a1fc-126">String</span></span>|<span data-ttu-id="8a1fc-127">O identificador do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="8a1fc-128">displayName</span><span class="sxs-lookup"><span data-stu-id="8a1fc-128">displayName</span></span>|<span data-ttu-id="8a1fc-129">String</span><span class="sxs-lookup"><span data-stu-id="8a1fc-129">String</span></span>|<span data-ttu-id="8a1fc-130">O nome de exibição da chave conforme dado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="8a1fc-131">creationDateTime</span><span class="sxs-lookup"><span data-stu-id="8a1fc-131">creationDateTime</span></span>|<span data-ttu-id="8a1fc-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8a1fc-132">DateTimeOffset</span></span>|<span data-ttu-id="8a1fc-133">O timestamp quando essa chave foi registrada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="8a1fc-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="8a1fc-134">aaGuid</span></span>|<span data-ttu-id="8a1fc-135">String</span><span class="sxs-lookup"><span data-stu-id="8a1fc-135">String</span></span>|<span data-ttu-id="8a1fc-136">GUID de Atestado de Autenticador, um identificador que indica o tipo (por exemplo, make e model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="8a1fc-137">modelo</span><span class="sxs-lookup"><span data-stu-id="8a1fc-137">model</span></span>|<span data-ttu-id="8a1fc-138">String</span><span class="sxs-lookup"><span data-stu-id="8a1fc-138">String</span></span>|<span data-ttu-id="8a1fc-139">O modelo atribuído pelo fabricante da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="8a1fc-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="8a1fc-140">attestationCertificates</span></span>|<span data-ttu-id="8a1fc-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="8a1fc-141">String collection</span></span>|<span data-ttu-id="8a1fc-142">Os certificados de atestado anexados a essa chave de segurança.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="8a1fc-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="8a1fc-143">attestationLevel</span></span>|<span data-ttu-id="8a1fc-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="8a1fc-144">attestationLevel</span></span>|<span data-ttu-id="8a1fc-145">O nível de atestado dessa chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="8a1fc-146">Os valores possíveis são: `attested` , ou `notAttested` .</span><span class="sxs-lookup"><span data-stu-id="8a1fc-146">Possible values are: `attested`, or `notAttested`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="8a1fc-147">Relações</span><span class="sxs-lookup"><span data-stu-id="8a1fc-147">Relationships</span></span>
<span data-ttu-id="8a1fc-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8a1fc-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8a1fc-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8a1fc-149">JSON representation</span></span>
<span data-ttu-id="8a1fc-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8a1fc-150">The following is a JSON representation of the resource.</span></span>
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

