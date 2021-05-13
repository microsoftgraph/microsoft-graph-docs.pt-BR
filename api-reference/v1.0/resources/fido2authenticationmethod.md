---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 1212f1e473d6f8bfe6ac06fbee0b96b12256a377
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335587"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="73bfd-104">Tipo de recurso fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73bfd-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="73bfd-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73bfd-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73bfd-106">Uma representação de uma chave de segurança FIDO2 registrada em um usuário.</span><span class="sxs-lookup"><span data-stu-id="73bfd-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="73bfd-107">FIDO2 é um método de autenticação de login.</span><span class="sxs-lookup"><span data-stu-id="73bfd-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="73bfd-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="73bfd-108">Methods</span></span>
|<span data-ttu-id="73bfd-109">Método</span><span class="sxs-lookup"><span data-stu-id="73bfd-109">Method</span></span>|<span data-ttu-id="73bfd-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="73bfd-110">Return type</span></span>|<span data-ttu-id="73bfd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bfd-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="73bfd-112">List</span><span class="sxs-lookup"><span data-stu-id="73bfd-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="73bfd-113">[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="73bfd-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="73bfd-114">Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="73bfd-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="73bfd-115">Get</span><span class="sxs-lookup"><span data-stu-id="73bfd-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="73bfd-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="73bfd-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="73bfd-117">Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="73bfd-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="73bfd-118">Delete</span><span class="sxs-lookup"><span data-stu-id="73bfd-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="73bfd-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73bfd-119">None</span></span>|<span data-ttu-id="73bfd-120">Exclui o objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="73bfd-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="73bfd-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="73bfd-121">Properties</span></span>
|<span data-ttu-id="73bfd-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="73bfd-122">Property</span></span>|<span data-ttu-id="73bfd-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="73bfd-123">Type</span></span>|<span data-ttu-id="73bfd-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="73bfd-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73bfd-125">id</span><span class="sxs-lookup"><span data-stu-id="73bfd-125">id</span></span>|<span data-ttu-id="73bfd-126">String</span><span class="sxs-lookup"><span data-stu-id="73bfd-126">String</span></span>|<span data-ttu-id="73bfd-127">O identificador do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="73bfd-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="73bfd-128">displayName</span><span class="sxs-lookup"><span data-stu-id="73bfd-128">displayName</span></span>|<span data-ttu-id="73bfd-129">String</span><span class="sxs-lookup"><span data-stu-id="73bfd-129">String</span></span>|<span data-ttu-id="73bfd-130">O nome de exibição da chave conforme dado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="73bfd-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="73bfd-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="73bfd-131">createdDateTime</span></span>|<span data-ttu-id="73bfd-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73bfd-132">DateTimeOffset</span></span>|<span data-ttu-id="73bfd-133">O timestamp quando essa chave foi registrada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="73bfd-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="73bfd-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="73bfd-134">aaGuid</span></span>|<span data-ttu-id="73bfd-135">String</span><span class="sxs-lookup"><span data-stu-id="73bfd-135">String</span></span>|<span data-ttu-id="73bfd-136">Authenticator GUID de atestado, um identificador que indica o tipo (por exemplo, make e model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="73bfd-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="73bfd-137">modelo</span><span class="sxs-lookup"><span data-stu-id="73bfd-137">model</span></span>|<span data-ttu-id="73bfd-138">String</span><span class="sxs-lookup"><span data-stu-id="73bfd-138">String</span></span>|<span data-ttu-id="73bfd-139">O modelo atribuído pelo fabricante da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="73bfd-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="73bfd-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="73bfd-140">attestationCertificates</span></span>|<span data-ttu-id="73bfd-141">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="73bfd-141">String collection</span></span>|<span data-ttu-id="73bfd-142">Os certificados de atestado anexados a essa chave de segurança.</span><span class="sxs-lookup"><span data-stu-id="73bfd-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="73bfd-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="73bfd-143">attestationLevel</span></span>|<span data-ttu-id="73bfd-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="73bfd-144">attestationLevel</span></span>|<span data-ttu-id="73bfd-145">O nível de atestado dessa chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="73bfd-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="73bfd-146">Os valores possíveis são: `attested` , ou `notAttested` .</span><span class="sxs-lookup"><span data-stu-id="73bfd-146">Possible values are: `attested`, or `notAttested`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="73bfd-147">Relações</span><span class="sxs-lookup"><span data-stu-id="73bfd-147">Relationships</span></span>
<span data-ttu-id="73bfd-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="73bfd-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="73bfd-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="73bfd-149">JSON representation</span></span>
<span data-ttu-id="73bfd-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="73bfd-150">The following is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

