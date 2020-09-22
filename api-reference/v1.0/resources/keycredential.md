---
title: tipo de recurso keycredential
description: Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço. A propriedade **Keycredentials** do aplicativo e das entidades do servicePrincipalName é uma coleção de **keycredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 97aab57c1ed0aa9f43536b89b49ca93a422962da
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48072932"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="7a0e0-104">tipo de recurso keycredential</span><span class="sxs-lookup"><span data-stu-id="7a0e0-104">keyCredential resource type</span></span>

<span data-ttu-id="7a0e0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7a0e0-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7a0e0-106">Contém uma credencial de chave associada a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="7a0e0-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="7a0e0-107">.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-107">.</span></span> <span data-ttu-id="7a0e0-108">A propriedade **Keycredentials** do [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="7a0e0-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="7a0e0-109">Entity é uma coleção de **keycredential**.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="7a0e0-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="7a0e0-110">Properties</span></span>
| <span data-ttu-id="7a0e0-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7a0e0-111">Property</span></span>     | <span data-ttu-id="7a0e0-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="7a0e0-112">Type</span></span>   |<span data-ttu-id="7a0e0-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="7a0e0-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7a0e0-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="7a0e0-114">customKeyIdentifier</span></span>|<span data-ttu-id="7a0e0-115">Binária</span><span class="sxs-lookup"><span data-stu-id="7a0e0-115">Binary</span></span>| <span data-ttu-id="7a0e0-116">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="7a0e0-116">Custom key identifier</span></span> |
| <span data-ttu-id="7a0e0-117">displayName</span><span class="sxs-lookup"><span data-stu-id="7a0e0-117">displayName</span></span> | <span data-ttu-id="7a0e0-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a0e0-118">String</span></span> | <span data-ttu-id="7a0e0-119">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-119">Friendly name for the key.</span></span> <span data-ttu-id="7a0e0-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-120">Optional.</span></span> |
|<span data-ttu-id="7a0e0-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7a0e0-121">endDateTime</span></span>|<span data-ttu-id="7a0e0-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a0e0-122">DateTimeOffset</span></span>|<span data-ttu-id="7a0e0-123">A data e a hora em que a credencial expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a0e0-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7a0e0-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7a0e0-125">keyId</span><span class="sxs-lookup"><span data-stu-id="7a0e0-125">keyId</span></span>|<span data-ttu-id="7a0e0-126">Guid</span><span class="sxs-lookup"><span data-stu-id="7a0e0-126">Guid</span></span>|<span data-ttu-id="7a0e0-127">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="7a0e0-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7a0e0-128">startDateTime</span></span>|<span data-ttu-id="7a0e0-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7a0e0-129">DateTimeOffset</span></span>|<span data-ttu-id="7a0e0-130">A data e a hora em que a credencial se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7a0e0-131">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7a0e0-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7a0e0-132">type</span><span class="sxs-lookup"><span data-stu-id="7a0e0-132">type</span></span>|<span data-ttu-id="7a0e0-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a0e0-133">String</span></span>|<span data-ttu-id="7a0e0-134">O tipo de credencial de chave; por exemplo, "simétrico".</span><span class="sxs-lookup"><span data-stu-id="7a0e0-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="7a0e0-135">ocorrência</span><span class="sxs-lookup"><span data-stu-id="7a0e0-135">usage</span></span>|<span data-ttu-id="7a0e0-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7a0e0-136">String</span></span>|<span data-ttu-id="7a0e0-137">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="7a0e0-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="7a0e0-138">chave</span><span class="sxs-lookup"><span data-stu-id="7a0e0-138">key</span></span>|<span data-ttu-id="7a0e0-139">Binário</span><span class="sxs-lookup"><span data-stu-id="7a0e0-139">Binary</span></span>| <span data-ttu-id="7a0e0-140">Valor para a credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-140">Value for the key credential.</span></span> <span data-ttu-id="7a0e0-141">Deve ser um valor codificado de base 64.</span><span class="sxs-lookup"><span data-stu-id="7a0e0-141">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7a0e0-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="7a0e0-142">JSON representation</span></span>

<span data-ttu-id="7a0e0-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="7a0e0-143">Here is a JSON representation of the resource</span></span>

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

