---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou entidade de serviço. A **propriedade keyCredentials** do aplicativo e entidades servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 7ba1bfbf5a3769163a2e9c839b568f22f33f9ac8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135433"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="4a0c0-104">Tipo de recurso keyCredential</span><span class="sxs-lookup"><span data-stu-id="4a0c0-104">keyCredential resource type</span></span>

<span data-ttu-id="4a0c0-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4a0c0-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4a0c0-106">Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="4a0c0-107">A **propriedade keyCredentials** do [aplicativo e](application.md) [entidades servicePrincipal](serviceprincipal.md) é uma coleção de **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="4a0c0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4a0c0-108">Properties</span></span>
| <span data-ttu-id="4a0c0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a0c0-109">Property</span></span>     | <span data-ttu-id="4a0c0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a0c0-110">Type</span></span>   |<span data-ttu-id="4a0c0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a0c0-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4a0c0-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="4a0c0-112">customKeyIdentifier</span></span>|<span data-ttu-id="4a0c0-113">Binária</span><span class="sxs-lookup"><span data-stu-id="4a0c0-113">Binary</span></span>| <span data-ttu-id="4a0c0-114">Identificador de chave personalizado</span><span class="sxs-lookup"><span data-stu-id="4a0c0-114">Custom key identifier</span></span> |
| <span data-ttu-id="4a0c0-115">displayName</span><span class="sxs-lookup"><span data-stu-id="4a0c0-115">displayName</span></span> | <span data-ttu-id="4a0c0-116">String</span><span class="sxs-lookup"><span data-stu-id="4a0c0-116">String</span></span> | <span data-ttu-id="4a0c0-117">Nome amigável da chave.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-117">Friendly name for the key.</span></span> <span data-ttu-id="4a0c0-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-118">Optional.</span></span> |
|<span data-ttu-id="4a0c0-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="4a0c0-119">endDateTime</span></span>|<span data-ttu-id="4a0c0-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a0c0-120">DateTimeOffset</span></span>|<span data-ttu-id="4a0c0-121">A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a0c0-122">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4a0c0-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4a0c0-123">keyId</span><span class="sxs-lookup"><span data-stu-id="4a0c0-123">keyId</span></span>|<span data-ttu-id="4a0c0-124">Guid</span><span class="sxs-lookup"><span data-stu-id="4a0c0-124">Guid</span></span>|<span data-ttu-id="4a0c0-125">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="4a0c0-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="4a0c0-126">startDateTime</span></span>|<span data-ttu-id="4a0c0-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4a0c0-127">DateTimeOffset</span></span>|<span data-ttu-id="4a0c0-128">A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="4a0c0-129">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="4a0c0-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="4a0c0-130">type</span><span class="sxs-lookup"><span data-stu-id="4a0c0-130">type</span></span>|<span data-ttu-id="4a0c0-131">String</span><span class="sxs-lookup"><span data-stu-id="4a0c0-131">String</span></span>|<span data-ttu-id="4a0c0-132">O tipo de credencial de chave; por exemplo, "Simétrico".</span><span class="sxs-lookup"><span data-stu-id="4a0c0-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="4a0c0-133">usage</span><span class="sxs-lookup"><span data-stu-id="4a0c0-133">usage</span></span>|<span data-ttu-id="4a0c0-134">String</span><span class="sxs-lookup"><span data-stu-id="4a0c0-134">String</span></span>|<span data-ttu-id="4a0c0-135">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="4a0c0-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="4a0c0-136">chave</span><span class="sxs-lookup"><span data-stu-id="4a0c0-136">key</span></span>|<span data-ttu-id="4a0c0-137">Binário</span><span class="sxs-lookup"><span data-stu-id="4a0c0-137">Binary</span></span>| <span data-ttu-id="4a0c0-138">Valor da credencial da chave.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-138">Value for the key credential.</span></span> <span data-ttu-id="4a0c0-139">Deve ser um valor codificado em base 64.</span><span class="sxs-lookup"><span data-stu-id="4a0c0-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="4a0c0-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4a0c0-140">JSON representation</span></span>

<span data-ttu-id="4a0c0-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="4a0c0-141">Here is a JSON representation of the resource</span></span>

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


