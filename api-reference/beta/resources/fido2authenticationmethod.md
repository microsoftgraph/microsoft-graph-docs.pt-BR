---
title: Tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança FIDO2 registrada em um usuário. FIDO2 é um método de autenticação de login.
author: mmcla
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 87c7f5e0f9ed29e6e1f5aa7c8ec332620bcc8a0a
ms.sourcegitcommit: 2d8b04725ea4eaf304f3da1056a6451457a4630f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/12/2021
ms.locfileid: "52335643"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="76d7a-104">Tipo de recurso fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="76d7a-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="76d7a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="76d7a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="76d7a-106">Uma representação de uma chave de segurança FIDO2 registrada em um usuário.</span><span class="sxs-lookup"><span data-stu-id="76d7a-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="76d7a-107">FIDO2 é um método de autenticação de login.</span><span class="sxs-lookup"><span data-stu-id="76d7a-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="76d7a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="76d7a-108">Methods</span></span>
|<span data-ttu-id="76d7a-109">Método</span><span class="sxs-lookup"><span data-stu-id="76d7a-109">Method</span></span>|<span data-ttu-id="76d7a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="76d7a-110">Return type</span></span>|<span data-ttu-id="76d7a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="76d7a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="76d7a-112">List</span><span class="sxs-lookup"><span data-stu-id="76d7a-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="76d7a-113">[coleção fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="76d7a-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="76d7a-114">Recupere uma lista dos objetos fido2AuthenticationMethod de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="76d7a-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="76d7a-115">Get</span><span class="sxs-lookup"><span data-stu-id="76d7a-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="76d7a-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="76d7a-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="76d7a-117">Leia as propriedades e as relações do objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="76d7a-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="76d7a-118">Delete</span><span class="sxs-lookup"><span data-stu-id="76d7a-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="76d7a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d7a-119">None</span></span>|<span data-ttu-id="76d7a-120">Exclui o objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="76d7a-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="76d7a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="76d7a-121">Properties</span></span>
|<span data-ttu-id="76d7a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="76d7a-122">Property</span></span>|<span data-ttu-id="76d7a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="76d7a-123">Type</span></span>|<span data-ttu-id="76d7a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="76d7a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76d7a-125">id</span><span class="sxs-lookup"><span data-stu-id="76d7a-125">id</span></span>|<span data-ttu-id="76d7a-126">String</span><span class="sxs-lookup"><span data-stu-id="76d7a-126">String</span></span>|<span data-ttu-id="76d7a-127">O identificador do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="76d7a-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="76d7a-128">displayName</span><span class="sxs-lookup"><span data-stu-id="76d7a-128">displayName</span></span>|<span data-ttu-id="76d7a-129">String</span><span class="sxs-lookup"><span data-stu-id="76d7a-129">String</span></span>|<span data-ttu-id="76d7a-130">O nome de exibição da chave conforme dado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="76d7a-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="76d7a-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="76d7a-131">createdDateTime</span></span>|<span data-ttu-id="76d7a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76d7a-132">DateTimeOffset</span></span>|<span data-ttu-id="76d7a-133">O timestamp quando essa chave foi registrada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="76d7a-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="76d7a-134">creationDateTime (Preterido)</span><span class="sxs-lookup"><span data-stu-id="76d7a-134">creationDateTime (Deprecated)</span></span>|<span data-ttu-id="76d7a-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="76d7a-135">DateTimeOffset</span></span>|<span data-ttu-id="76d7a-136">O timestamp quando essa chave foi registrada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="76d7a-136">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="76d7a-137">aaGuid</span><span class="sxs-lookup"><span data-stu-id="76d7a-137">aaGuid</span></span>|<span data-ttu-id="76d7a-138">String</span><span class="sxs-lookup"><span data-stu-id="76d7a-138">String</span></span>|<span data-ttu-id="76d7a-139">Authenticator GUID de atestado, um identificador que indica o tipo (por exemplo, make e model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="76d7a-139">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="76d7a-140">modelo</span><span class="sxs-lookup"><span data-stu-id="76d7a-140">model</span></span>|<span data-ttu-id="76d7a-141">String</span><span class="sxs-lookup"><span data-stu-id="76d7a-141">String</span></span>|<span data-ttu-id="76d7a-142">O modelo atribuído pelo fabricante da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="76d7a-142">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="76d7a-143">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="76d7a-143">attestationCertificates</span></span>|<span data-ttu-id="76d7a-144">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="76d7a-144">String collection</span></span>|<span data-ttu-id="76d7a-145">Os certificados de atestado anexados a essa chave de segurança.</span><span class="sxs-lookup"><span data-stu-id="76d7a-145">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="76d7a-146">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="76d7a-146">attestationLevel</span></span>|<span data-ttu-id="76d7a-147">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="76d7a-147">attestationLevel</span></span>|<span data-ttu-id="76d7a-148">O nível de atestado dessa chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="76d7a-148">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="76d7a-149">Os valores possíveis são: `attested`, `notAttested`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="76d7a-149">Possible values are: `attested`, `notAttested`, `unknownFutureValue`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="76d7a-150">Relações</span><span class="sxs-lookup"><span data-stu-id="76d7a-150">Relationships</span></span>
<span data-ttu-id="76d7a-151">Nenhum</span><span class="sxs-lookup"><span data-stu-id="76d7a-151">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="76d7a-152">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="76d7a-152">JSON representation</span></span>
<span data-ttu-id="76d7a-153">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="76d7a-153">The following is a JSON representation of the resource.</span></span>
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
  "createdDateTime": "String (timestamp)",
  "aaGuid": "String",
  "model": "String",
  "attestationCertificates": [
    "String"
  ],
  "attestationLevel": "String"
}
```

