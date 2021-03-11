---
title: Tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A **propriedade keyCredentials** das entidades application and servicePrincipal é uma coleção de **keyCredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: cc6d66a4361f760b702844991e6fdc3f590c4007
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721485"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="ff274-104">Tipo de recurso keyCredential</span><span class="sxs-lookup"><span data-stu-id="ff274-104">keyCredential resource type</span></span>

<span data-ttu-id="ff274-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff274-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff274-106">Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="ff274-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="ff274-107">A **propriedade keyCredentials** das entidades [application](application.md) and [servicePrincipal](serviceprincipal.md) é uma coleção **de keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="ff274-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="ff274-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff274-108">Properties</span></span>
| <span data-ttu-id="ff274-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff274-109">Property</span></span>     | <span data-ttu-id="ff274-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff274-110">Type</span></span>   |<span data-ttu-id="ff274-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff274-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ff274-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="ff274-112">customKeyIdentifier</span></span>|<span data-ttu-id="ff274-113">Binária</span><span class="sxs-lookup"><span data-stu-id="ff274-113">Binary</span></span>| <span data-ttu-id="ff274-114">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="ff274-114">Custom key identifier</span></span> |
| <span data-ttu-id="ff274-115">displayName</span><span class="sxs-lookup"><span data-stu-id="ff274-115">displayName</span></span> | <span data-ttu-id="ff274-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff274-116">String</span></span> | <span data-ttu-id="ff274-117">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="ff274-117">Friendly name for the key.</span></span> <span data-ttu-id="ff274-118">Opcional.</span><span class="sxs-lookup"><span data-stu-id="ff274-118">Optional.</span></span> |
|<span data-ttu-id="ff274-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ff274-119">endDateTime</span></span>|<span data-ttu-id="ff274-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff274-120">DateTimeOffset</span></span>|<span data-ttu-id="ff274-121">A data e a hora em que a credencial expira. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ff274-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ff274-122">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ff274-122">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ff274-123">keyId</span><span class="sxs-lookup"><span data-stu-id="ff274-123">keyId</span></span>|<span data-ttu-id="ff274-124">Guid</span><span class="sxs-lookup"><span data-stu-id="ff274-124">Guid</span></span>|<span data-ttu-id="ff274-125">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="ff274-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="ff274-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ff274-126">startDateTime</span></span>|<span data-ttu-id="ff274-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff274-127">DateTimeOffset</span></span>|<span data-ttu-id="ff274-128">A data e a hora em que a credencial se torna válida. O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ff274-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ff274-129">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="ff274-129">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="ff274-130">tipo</span><span class="sxs-lookup"><span data-stu-id="ff274-130">type</span></span>|<span data-ttu-id="ff274-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff274-131">String</span></span>|<span data-ttu-id="ff274-132">O tipo de credencial de chave; por exemplo, "Simétrico".</span><span class="sxs-lookup"><span data-stu-id="ff274-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="ff274-133">usage</span><span class="sxs-lookup"><span data-stu-id="ff274-133">usage</span></span>|<span data-ttu-id="ff274-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff274-134">String</span></span>|<span data-ttu-id="ff274-135">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="ff274-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="ff274-136">chave</span><span class="sxs-lookup"><span data-stu-id="ff274-136">key</span></span>|<span data-ttu-id="ff274-137">Binário</span><span class="sxs-lookup"><span data-stu-id="ff274-137">Binary</span></span>| <span data-ttu-id="ff274-138">Valor para a credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="ff274-138">Value for the key credential.</span></span> <span data-ttu-id="ff274-139">Deve ser um valor codificado base 64.</span><span class="sxs-lookup"><span data-stu-id="ff274-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ff274-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff274-140">JSON representation</span></span>

<span data-ttu-id="ff274-141">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ff274-141">Here is a JSON representation of the resource</span></span>

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


