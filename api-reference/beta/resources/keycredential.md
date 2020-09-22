---
title: tipo de recurso keycredential
description: Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço. A propriedade **Keycredentials** do aplicativo e das entidades do servicePrincipalName é uma coleção de **keycredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 6c005a44827640ed7a61e61f07837a98021d9a9c
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078336"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="adccf-104">tipo de recurso keycredential</span><span class="sxs-lookup"><span data-stu-id="adccf-104">keyCredential resource type</span></span>

<span data-ttu-id="adccf-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="adccf-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="adccf-106">Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="adccf-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="adccf-107">A propriedade **Keycredentials** do [aplicativo](application.md) e das entidades do [servicePrincipalName](serviceprincipal.md) é uma coleção de **keycredential**.</span><span class="sxs-lookup"><span data-stu-id="adccf-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="adccf-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="adccf-108">Properties</span></span>
| <span data-ttu-id="adccf-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="adccf-109">Property</span></span>     | <span data-ttu-id="adccf-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="adccf-110">Type</span></span>   |<span data-ttu-id="adccf-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="adccf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="adccf-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="adccf-112">customKeyIdentifier</span></span>|<span data-ttu-id="adccf-113">Binária</span><span class="sxs-lookup"><span data-stu-id="adccf-113">Binary</span></span>| <span data-ttu-id="adccf-114">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="adccf-114">Custom key identifier</span></span> |
| <span data-ttu-id="adccf-115">displayName</span><span class="sxs-lookup"><span data-stu-id="adccf-115">displayName</span></span> | <span data-ttu-id="adccf-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adccf-116">String</span></span> | <span data-ttu-id="adccf-117">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="adccf-117">Friendly name for the key.</span></span> <span data-ttu-id="adccf-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="adccf-118">Optional.</span></span> |
|<span data-ttu-id="adccf-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="adccf-119">endDateTime</span></span>|<span data-ttu-id="adccf-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adccf-120">DateTimeOffset</span></span>|<span data-ttu-id="adccf-121">A data e a hora em que a credencial expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="adccf-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adccf-122">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="adccf-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="adccf-123">keyId</span><span class="sxs-lookup"><span data-stu-id="adccf-123">keyId</span></span>|<span data-ttu-id="adccf-124">Guid</span><span class="sxs-lookup"><span data-stu-id="adccf-124">Guid</span></span>|<span data-ttu-id="adccf-125">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="adccf-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="adccf-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="adccf-126">startDateTime</span></span>|<span data-ttu-id="adccf-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="adccf-127">DateTimeOffset</span></span>|<span data-ttu-id="adccf-128">A data e a hora em que a credencial se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="adccf-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="adccf-129">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="adccf-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="adccf-130">tipo</span><span class="sxs-lookup"><span data-stu-id="adccf-130">type</span></span>|<span data-ttu-id="adccf-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adccf-131">String</span></span>|<span data-ttu-id="adccf-132">O tipo de credencial de chave; por exemplo, "simétrico".</span><span class="sxs-lookup"><span data-stu-id="adccf-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="adccf-133">ocorrência</span><span class="sxs-lookup"><span data-stu-id="adccf-133">usage</span></span>|<span data-ttu-id="adccf-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="adccf-134">String</span></span>|<span data-ttu-id="adccf-135">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="adccf-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="adccf-136">chave</span><span class="sxs-lookup"><span data-stu-id="adccf-136">key</span></span>|<span data-ttu-id="adccf-137">Binário</span><span class="sxs-lookup"><span data-stu-id="adccf-137">Binary</span></span>| <span data-ttu-id="adccf-138">Valor para a credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="adccf-138">Value for the key credential.</span></span> <span data-ttu-id="adccf-139">Deve ser um valor codificado de base 64.</span><span class="sxs-lookup"><span data-stu-id="adccf-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="adccf-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="adccf-140">JSON representation</span></span>

<span data-ttu-id="adccf-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="adccf-141">Here is a JSON representation of the resource</span></span>

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


