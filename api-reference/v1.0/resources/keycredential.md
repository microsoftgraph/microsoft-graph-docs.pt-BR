---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials** das entidades application and servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 05b0aa71059bcf0ef974e49fb012a3815386b9be
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722234"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="24672-104">Tipo de recurso keyCredential</span><span class="sxs-lookup"><span data-stu-id="24672-104">keyCredential resource type</span></span>

<span data-ttu-id="24672-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24672-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24672-106">Contém uma credencial de chave associada a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="24672-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="24672-107">.</span><span class="sxs-lookup"><span data-stu-id="24672-107">.</span></span> <span data-ttu-id="24672-108">A **propriedade keyCredentials** do [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="24672-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="24672-109">entity é uma coleção de **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="24672-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="24672-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="24672-110">Properties</span></span>
| <span data-ttu-id="24672-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="24672-111">Property</span></span>     | <span data-ttu-id="24672-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="24672-112">Type</span></span>   |<span data-ttu-id="24672-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="24672-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="24672-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="24672-114">customKeyIdentifier</span></span>|<span data-ttu-id="24672-115">Binária</span><span class="sxs-lookup"><span data-stu-id="24672-115">Binary</span></span>| <span data-ttu-id="24672-116">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="24672-116">Custom key identifier</span></span> |
| <span data-ttu-id="24672-117">displayName</span><span class="sxs-lookup"><span data-stu-id="24672-117">displayName</span></span> | <span data-ttu-id="24672-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24672-118">String</span></span> | <span data-ttu-id="24672-119">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="24672-119">Friendly name for the key.</span></span> <span data-ttu-id="24672-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="24672-120">Optional.</span></span> |
|<span data-ttu-id="24672-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="24672-121">endDateTime</span></span>|<span data-ttu-id="24672-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24672-122">DateTimeOffset</span></span>|<span data-ttu-id="24672-123">A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="24672-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24672-124">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="24672-124">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="24672-125">keyId</span><span class="sxs-lookup"><span data-stu-id="24672-125">keyId</span></span>|<span data-ttu-id="24672-126">Guid</span><span class="sxs-lookup"><span data-stu-id="24672-126">Guid</span></span>|<span data-ttu-id="24672-127">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="24672-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="24672-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="24672-128">startDateTime</span></span>|<span data-ttu-id="24672-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="24672-129">DateTimeOffset</span></span>|<span data-ttu-id="24672-130">A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="24672-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="24672-131">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="24672-131">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="24672-132">tipo</span><span class="sxs-lookup"><span data-stu-id="24672-132">type</span></span>|<span data-ttu-id="24672-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24672-133">String</span></span>|<span data-ttu-id="24672-134">O tipo de credencial de chave; por exemplo, "Simétrico".</span><span class="sxs-lookup"><span data-stu-id="24672-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="24672-135">usage</span><span class="sxs-lookup"><span data-stu-id="24672-135">usage</span></span>|<span data-ttu-id="24672-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="24672-136">String</span></span>|<span data-ttu-id="24672-137">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="24672-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="24672-138">chave</span><span class="sxs-lookup"><span data-stu-id="24672-138">key</span></span>|<span data-ttu-id="24672-139">Binário</span><span class="sxs-lookup"><span data-stu-id="24672-139">Binary</span></span>| <span data-ttu-id="24672-140">Os dados brutos do certificado na matriz de byte convertidos na cadeia de caracteres Base64; por exemplo, `[System.Convert]::ToBase64String($Cert.GetRawCertData())` .</span><span class="sxs-lookup"><span data-stu-id="24672-140">The certificate's raw data in byte array converted to Base64 string; for example, `[System.Convert]::ToBase64String($Cert.GetRawCertData())`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="24672-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="24672-141">JSON representation</span></span>

<span data-ttu-id="24672-142">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="24672-142">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

