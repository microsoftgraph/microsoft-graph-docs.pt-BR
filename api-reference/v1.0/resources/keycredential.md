---
title: tipo de recurso keycredential
description: Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço. A propriedade **Keycredentials** do aplicativo e das entidades do servicePrincipalName é uma coleção de **keycredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 346ff30ad0479d2b25dc57d09a67cc4ddd5f83bc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939625"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="b62bb-104">tipo de recurso keycredential</span><span class="sxs-lookup"><span data-stu-id="b62bb-104">keyCredential resource type</span></span>

<span data-ttu-id="b62bb-105">Contém uma credencial de chave associada a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="b62bb-105">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="b62bb-106">.</span><span class="sxs-lookup"><span data-stu-id="b62bb-106"></span></span> <span data-ttu-id="b62bb-107">A propriedade **Keycredentials** do [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="b62bb-107">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="b62bb-108">Entity é uma coleção de **keycredential**.</span><span class="sxs-lookup"><span data-stu-id="b62bb-108">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="b62bb-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b62bb-109">Properties</span></span>
| <span data-ttu-id="b62bb-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b62bb-110">Property</span></span>     | <span data-ttu-id="b62bb-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="b62bb-111">Type</span></span>   |<span data-ttu-id="b62bb-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="b62bb-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b62bb-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="b62bb-113">customKeyIdentifier</span></span>|<span data-ttu-id="b62bb-114">Binária</span><span class="sxs-lookup"><span data-stu-id="b62bb-114">Binary</span></span>| <span data-ttu-id="b62bb-115">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="b62bb-115">Custom key identifier</span></span> |
| <span data-ttu-id="b62bb-116">displayName</span><span class="sxs-lookup"><span data-stu-id="b62bb-116">displayName</span></span> | <span data-ttu-id="b62bb-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b62bb-117">String</span></span> | <span data-ttu-id="b62bb-118">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="b62bb-118">Friendly name for the key.</span></span> <span data-ttu-id="b62bb-119">Opcional.</span><span class="sxs-lookup"><span data-stu-id="b62bb-119">Optional.</span></span> |
|<span data-ttu-id="b62bb-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="b62bb-120">endDateTime</span></span>|<span data-ttu-id="b62bb-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b62bb-121">DateTimeOffset</span></span>|<span data-ttu-id="b62bb-122">A data e a hora em que a credencial expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b62bb-122">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b62bb-123">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b62bb-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b62bb-124">keyId</span><span class="sxs-lookup"><span data-stu-id="b62bb-124">keyId</span></span>|<span data-ttu-id="b62bb-125">Guid</span><span class="sxs-lookup"><span data-stu-id="b62bb-125">Guid</span></span>|<span data-ttu-id="b62bb-126">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="b62bb-126">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="b62bb-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="b62bb-127">startDateTime</span></span>|<span data-ttu-id="b62bb-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b62bb-128">DateTimeOffset</span></span>|<span data-ttu-id="b62bb-129">A data e a hora em que a credencial se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b62bb-129">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b62bb-130">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b62bb-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b62bb-131">type</span><span class="sxs-lookup"><span data-stu-id="b62bb-131">type</span></span>|<span data-ttu-id="b62bb-132">String</span><span class="sxs-lookup"><span data-stu-id="b62bb-132">String</span></span>|<span data-ttu-id="b62bb-133">O tipo de credencial de chave; por exemplo, "simétrico".</span><span class="sxs-lookup"><span data-stu-id="b62bb-133">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="b62bb-134">ocorrência</span><span class="sxs-lookup"><span data-stu-id="b62bb-134">usage</span></span>|<span data-ttu-id="b62bb-135">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b62bb-135">String</span></span>|<span data-ttu-id="b62bb-136">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="b62bb-136">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="b62bb-137">chave</span><span class="sxs-lookup"><span data-stu-id="b62bb-137">key</span></span>|<span data-ttu-id="b62bb-138">Binário</span><span class="sxs-lookup"><span data-stu-id="b62bb-138">Binary</span></span>| <span data-ttu-id="b62bb-139">Valor para a credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="b62bb-139">Value for the key credential.</span></span> <span data-ttu-id="b62bb-140">Deve ser um valor codificado de base 64.</span><span class="sxs-lookup"><span data-stu-id="b62bb-140">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b62bb-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b62bb-141">JSON representation</span></span>

<span data-ttu-id="b62bb-142">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="b62bb-142">Here is a JSON representation of the resource</span></span>

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
