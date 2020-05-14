---
title: tipo de recurso keycredential
description: Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço. A propriedade **Keycredentials** do aplicativo e das entidades do servicePrincipalName é uma coleção de **keycredential**.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 40837844b7ab78f86cd57438adeb08ceb97d52ad
ms.sourcegitcommit: d4114bac58628527611e83e436132c6581a19c52
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/13/2020
ms.locfileid: "43441493"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="2439f-104">tipo de recurso keycredential</span><span class="sxs-lookup"><span data-stu-id="2439f-104">keyCredential resource type</span></span>

<span data-ttu-id="2439f-105">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2439f-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2439f-106">Contém uma credencial de chave associada a um aplicativo</span><span class="sxs-lookup"><span data-stu-id="2439f-106">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="2439f-107">.</span><span class="sxs-lookup"><span data-stu-id="2439f-107">.</span></span> <span data-ttu-id="2439f-108">A propriedade **Keycredentials** do [aplicativo](application.md)</span><span class="sxs-lookup"><span data-stu-id="2439f-108">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="2439f-109">Entity é uma coleção de **keycredential**.</span><span class="sxs-lookup"><span data-stu-id="2439f-109">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="2439f-110">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2439f-110">Properties</span></span>
| <span data-ttu-id="2439f-111">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2439f-111">Property</span></span>     | <span data-ttu-id="2439f-112">Tipo</span><span class="sxs-lookup"><span data-stu-id="2439f-112">Type</span></span>   |<span data-ttu-id="2439f-113">Descrição</span><span class="sxs-lookup"><span data-stu-id="2439f-113">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2439f-114">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="2439f-114">customKeyIdentifier</span></span>|<span data-ttu-id="2439f-115">Binária</span><span class="sxs-lookup"><span data-stu-id="2439f-115">Binary</span></span>| <span data-ttu-id="2439f-116">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="2439f-116">Custom key identifier</span></span> |
| <span data-ttu-id="2439f-117">displayName</span><span class="sxs-lookup"><span data-stu-id="2439f-117">displayName</span></span> | <span data-ttu-id="2439f-118">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2439f-118">String</span></span> | <span data-ttu-id="2439f-119">Nome amigável para a chave.</span><span class="sxs-lookup"><span data-stu-id="2439f-119">Friendly name for the key.</span></span> <span data-ttu-id="2439f-120">Opcional.</span><span class="sxs-lookup"><span data-stu-id="2439f-120">Optional.</span></span> |
|<span data-ttu-id="2439f-121">endDateTime</span><span class="sxs-lookup"><span data-stu-id="2439f-121">endDateTime</span></span>|<span data-ttu-id="2439f-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2439f-122">DateTimeOffset</span></span>|<span data-ttu-id="2439f-123">A data e a hora em que a credencial expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2439f-123">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2439f-124">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2439f-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2439f-125">keyId</span><span class="sxs-lookup"><span data-stu-id="2439f-125">keyId</span></span>|<span data-ttu-id="2439f-126">Guid</span><span class="sxs-lookup"><span data-stu-id="2439f-126">Guid</span></span>|<span data-ttu-id="2439f-127">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="2439f-127">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="2439f-128">startDateTime</span><span class="sxs-lookup"><span data-stu-id="2439f-128">startDateTime</span></span>|<span data-ttu-id="2439f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2439f-129">DateTimeOffset</span></span>|<span data-ttu-id="2439f-130">A data e a hora em que a credencial se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="2439f-130">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2439f-131">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2439f-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2439f-132">type</span><span class="sxs-lookup"><span data-stu-id="2439f-132">type</span></span>|<span data-ttu-id="2439f-133">String</span><span class="sxs-lookup"><span data-stu-id="2439f-133">String</span></span>|<span data-ttu-id="2439f-134">O tipo de credencial de chave; por exemplo, "simétrico".</span><span class="sxs-lookup"><span data-stu-id="2439f-134">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="2439f-135">ocorrência</span><span class="sxs-lookup"><span data-stu-id="2439f-135">usage</span></span>|<span data-ttu-id="2439f-136">String</span><span class="sxs-lookup"><span data-stu-id="2439f-136">String</span></span>|<span data-ttu-id="2439f-137">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="2439f-137">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="2439f-138">chave</span><span class="sxs-lookup"><span data-stu-id="2439f-138">key</span></span>|<span data-ttu-id="2439f-139">Binário</span><span class="sxs-lookup"><span data-stu-id="2439f-139">Binary</span></span>| <span data-ttu-id="2439f-140">Valor para a credencial de chave.</span><span class="sxs-lookup"><span data-stu-id="2439f-140">Value for the key credential.</span></span> <span data-ttu-id="2439f-141">Deve ser um valor codificado de base 64.</span><span class="sxs-lookup"><span data-stu-id="2439f-141">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2439f-142">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2439f-142">JSON representation</span></span>

<span data-ttu-id="2439f-143">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="2439f-143">Here is a JSON representation of the resource</span></span>

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
