---
title: tipo de recurso fido2AuthenticationMethod
description: Uma representação de uma chave de segurança do FIDO2 registrada para um usuário. FIDO2 é um método de autenticação de entrada.
author: mmcla
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c4d10252201781d1339e6baa26aea248429ae462
ms.sourcegitcommit: cfadc605014265e02b913bc77382025b0d156285
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/10/2020
ms.locfileid: "48418173"
---
# <a name="fido2authenticationmethod-resource-type"></a><span data-ttu-id="b257a-104">tipo de recurso fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b257a-104">fido2AuthenticationMethod resource type</span></span>

<span data-ttu-id="b257a-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b257a-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b257a-106">Uma representação de uma chave de segurança do FIDO2 registrada para um usuário.</span><span class="sxs-lookup"><span data-stu-id="b257a-106">A representation of a FIDO2 security key registered to a user.</span></span> <span data-ttu-id="b257a-107">FIDO2 é um método de autenticação de entrada.</span><span class="sxs-lookup"><span data-stu-id="b257a-107">FIDO2 is a sign-in authentication method.</span></span>


## <a name="methods"></a><span data-ttu-id="b257a-108">Métodos</span><span class="sxs-lookup"><span data-stu-id="b257a-108">Methods</span></span>
|<span data-ttu-id="b257a-109">Método</span><span class="sxs-lookup"><span data-stu-id="b257a-109">Method</span></span>|<span data-ttu-id="b257a-110">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="b257a-110">Return type</span></span>|<span data-ttu-id="b257a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="b257a-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b257a-112">List</span><span class="sxs-lookup"><span data-stu-id="b257a-112">List</span></span>](../api/fido2authenticationmethod-list.md)|<span data-ttu-id="b257a-113">coleção [fido2AuthenticationMethod](../resources/fido2authenticationmethod.md)</span><span class="sxs-lookup"><span data-stu-id="b257a-113">[fido2AuthenticationMethod](../resources/fido2authenticationmethod.md) collection</span></span>|<span data-ttu-id="b257a-114">Recupere uma lista de objetos fido2AuthenticationMethod de um usuário e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="b257a-114">Retrieve a list of a user's fido2AuthenticationMethod objects and their properties.</span></span>|
|[<span data-ttu-id="b257a-115">Obter</span><span class="sxs-lookup"><span data-stu-id="b257a-115">Get</span></span>](../api/fido2authenticationmethod-get.md)|[<span data-ttu-id="b257a-116">fido2AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="b257a-116">fido2AuthenticationMethod</span></span>](../resources/fido2authenticationmethod.md)|<span data-ttu-id="b257a-117">Leia as propriedades e os relacionamentos do objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b257a-117">Read the properties and relationships of a user's fido2AuthenticationMethod object.</span></span>|
|[<span data-ttu-id="b257a-118">Excluir</span><span class="sxs-lookup"><span data-stu-id="b257a-118">Delete</span></span>](../api/fido2authenticationmethod-delete.md)|<span data-ttu-id="b257a-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b257a-119">None</span></span>|<span data-ttu-id="b257a-120">Exclui o objeto fido2AuthenticationMethod de um usuário.</span><span class="sxs-lookup"><span data-stu-id="b257a-120">Deletes a user's fido2AuthenticationMethod object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b257a-121">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b257a-121">Properties</span></span>
|<span data-ttu-id="b257a-122">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b257a-122">Property</span></span>|<span data-ttu-id="b257a-123">Tipo</span><span class="sxs-lookup"><span data-stu-id="b257a-123">Type</span></span>|<span data-ttu-id="b257a-124">Descrição</span><span class="sxs-lookup"><span data-stu-id="b257a-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b257a-125">id</span><span class="sxs-lookup"><span data-stu-id="b257a-125">id</span></span>|<span data-ttu-id="b257a-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b257a-126">String</span></span>|<span data-ttu-id="b257a-127">O identificador do método de autenticação.</span><span class="sxs-lookup"><span data-stu-id="b257a-127">The authentication method identifier.</span></span>|
|<span data-ttu-id="b257a-128">displayName</span><span class="sxs-lookup"><span data-stu-id="b257a-128">displayName</span></span>|<span data-ttu-id="b257a-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b257a-129">String</span></span>|<span data-ttu-id="b257a-130">O nome de exibição da chave, conforme fornecido pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b257a-130">The display name of the key as given by the user.</span></span>|
|<span data-ttu-id="b257a-131">creationDatetime</span><span class="sxs-lookup"><span data-stu-id="b257a-131">creationDateTime</span></span>|<span data-ttu-id="b257a-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b257a-132">DateTimeOffset</span></span>|<span data-ttu-id="b257a-133">O carimbo de data/hora em que essa chave foi registrada para o usuário.</span><span class="sxs-lookup"><span data-stu-id="b257a-133">The timestamp when this key was registered to the user.</span></span>|
|<span data-ttu-id="b257a-134">aaGuid</span><span class="sxs-lookup"><span data-stu-id="b257a-134">aaGuid</span></span>|<span data-ttu-id="b257a-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b257a-135">String</span></span>|<span data-ttu-id="b257a-136">GUID de atestado de autenticador, um identificador que indica o tipo (por exemplo, Make e Model) do autenticador.</span><span class="sxs-lookup"><span data-stu-id="b257a-136">Authenticator Attestation GUID, an identifier that indicates the type (e.g. make and model) of the authenticator.</span></span>|
|<span data-ttu-id="b257a-137">modelo</span><span class="sxs-lookup"><span data-stu-id="b257a-137">model</span></span>|<span data-ttu-id="b257a-138">String</span><span class="sxs-lookup"><span data-stu-id="b257a-138">String</span></span>|<span data-ttu-id="b257a-139">O modelo atribuído pelo fabricante da chave de segurança FIDO2.</span><span class="sxs-lookup"><span data-stu-id="b257a-139">The manufacturer-assigned model of the FIDO2 security key.</span></span>|
|<span data-ttu-id="b257a-140">attestationCertificates</span><span class="sxs-lookup"><span data-stu-id="b257a-140">attestationCertificates</span></span>|<span data-ttu-id="b257a-141">Conjunto de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b257a-141">String collection</span></span>|<span data-ttu-id="b257a-142">Os certificados de atestado anexados a essa chave de segurança.</span><span class="sxs-lookup"><span data-stu-id="b257a-142">The attestation certificate(s) attached to this security key.</span></span>|
|<span data-ttu-id="b257a-143">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="b257a-143">attestationLevel</span></span>|<span data-ttu-id="b257a-144">attestationLevel</span><span class="sxs-lookup"><span data-stu-id="b257a-144">attestationLevel</span></span>|<span data-ttu-id="b257a-145">O nível de atestado dessa chave de segurança do FIDO2.</span><span class="sxs-lookup"><span data-stu-id="b257a-145">The attestation level of this FIDO2 security key.</span></span> <span data-ttu-id="b257a-146">Os valores possíveis são: `attested` , ou `notAttested` .</span><span class="sxs-lookup"><span data-stu-id="b257a-146">Possible values are: `attested`, or `notAttested`.</span></span>|


## <a name="relationships"></a><span data-ttu-id="b257a-147">Relações</span><span class="sxs-lookup"><span data-stu-id="b257a-147">Relationships</span></span>
<span data-ttu-id="b257a-148">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b257a-148">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b257a-149">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b257a-149">JSON representation</span></span>
<span data-ttu-id="b257a-150">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b257a-150">The following is a JSON representation of the resource.</span></span>
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

