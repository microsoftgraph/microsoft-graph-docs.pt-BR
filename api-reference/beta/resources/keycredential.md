---
title: tipo de recurso keycredential
description: Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço. A propriedade **Keycredentials** do aplicativo e das entidades do servicePrincipalName é uma coleção de **keycredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 57305e7e5767b8ad5454d7fd3a229be53489b5fd
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939254"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="777f6-104">tipo de recurso keycredential</span><span class="sxs-lookup"><span data-stu-id="777f6-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="777f6-105">Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="777f6-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="777f6-106">A propriedade **Keycredentials** do [aplicativo](application.md) e das entidades do [servicePrincipalName](serviceprincipal.md) é uma coleção de **keycredential**.</span><span class="sxs-lookup"><span data-stu-id="777f6-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="777f6-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="777f6-107">Properties</span></span>
| <span data-ttu-id="777f6-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="777f6-108">Property</span></span>     | <span data-ttu-id="777f6-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="777f6-109">Type</span></span>   |<span data-ttu-id="777f6-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="777f6-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="777f6-111">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="777f6-111">customKeyIdentifier</span></span>|<span data-ttu-id="777f6-112">Binária</span><span class="sxs-lookup"><span data-stu-id="777f6-112">Binary</span></span>| <span data-ttu-id="777f6-113">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="777f6-113">Custom key identifier</span></span> |
| <span data-ttu-id="777f6-114">displayName</span><span class="sxs-lookup"><span data-stu-id="777f6-114">displayName</span></span> | <span data-ttu-id="777f6-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="777f6-115">String</span></span> | <span data-ttu-id="777f6-116">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="777f6-116">Friendly name for the key.</span></span> <span data-ttu-id="777f6-117">Opcional.</span><span class="sxs-lookup"><span data-stu-id="777f6-117">Optional.</span></span> |
|<span data-ttu-id="777f6-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="777f6-118">endDateTime</span></span>|<span data-ttu-id="777f6-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="777f6-119">DateTimeOffset</span></span>|<span data-ttu-id="777f6-120">A data e a hora em que a credencial expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="777f6-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="777f6-121">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="777f6-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="777f6-122">keyId</span><span class="sxs-lookup"><span data-stu-id="777f6-122">keyId</span></span>|<span data-ttu-id="777f6-123">Guid</span><span class="sxs-lookup"><span data-stu-id="777f6-123">Guid</span></span>|<span data-ttu-id="777f6-124">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="777f6-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="777f6-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="777f6-125">startDateTime</span></span>|<span data-ttu-id="777f6-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="777f6-126">DateTimeOffset</span></span>|<span data-ttu-id="777f6-127">A data e a hora em que a credencial se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="777f6-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="777f6-128">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="777f6-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="777f6-129">type</span><span class="sxs-lookup"><span data-stu-id="777f6-129">type</span></span>|<span data-ttu-id="777f6-130">String</span><span class="sxs-lookup"><span data-stu-id="777f6-130">String</span></span>|<span data-ttu-id="777f6-131">O tipo de credencial de chave; por exemplo, "simétrico".</span><span class="sxs-lookup"><span data-stu-id="777f6-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="777f6-132">ocorrência</span><span class="sxs-lookup"><span data-stu-id="777f6-132">usage</span></span>|<span data-ttu-id="777f6-133">String</span><span class="sxs-lookup"><span data-stu-id="777f6-133">String</span></span>|<span data-ttu-id="777f6-134">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="777f6-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="777f6-135">chave</span><span class="sxs-lookup"><span data-stu-id="777f6-135">key</span></span>|<span data-ttu-id="777f6-136">Binário</span><span class="sxs-lookup"><span data-stu-id="777f6-136">Binary</span></span>| <span data-ttu-id="777f6-137">Valor para a credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="777f6-137">Value for the key credential.</span></span> <span data-ttu-id="777f6-138">Deve ser um valor codificado de base 64.</span><span class="sxs-lookup"><span data-stu-id="777f6-138">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="777f6-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="777f6-139">JSON representation</span></span>

<span data-ttu-id="777f6-140">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="777f6-140">Here is a JSON representation of the resource</span></span>

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
