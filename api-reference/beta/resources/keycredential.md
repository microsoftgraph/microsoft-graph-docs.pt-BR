---
title: tipo de recurso keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço. A **** Propriedade keycredentials do aplicativo e das entidades do servicePrincipalName é uma coleção de keycredential. ****
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562668"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="ac586-104">tipo de recurso keyCredential</span><span class="sxs-lookup"><span data-stu-id="ac586-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac586-105">Contém uma credencial de chave associada a um aplicativo ou a uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="ac586-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="ac586-106">A \*\*\*\* Propriedade keycredentials do [aplicativo](application.md) e das entidades do [servicePrincipalName](serviceprincipal.md) é uma coleção \*\*\*\* de keycredential.</span><span class="sxs-lookup"><span data-stu-id="ac586-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ac586-107">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ac586-107">JSON representation</span></span>

<span data-ttu-id="ac586-108">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="ac586-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="ac586-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ac586-109">Properties</span></span>
| <span data-ttu-id="ac586-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ac586-110">Property</span></span>     | <span data-ttu-id="ac586-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ac586-111">Type</span></span>   |<span data-ttu-id="ac586-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ac586-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac586-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="ac586-113">customKeyIdentifier</span></span>|<span data-ttu-id="ac586-114">Binário</span><span class="sxs-lookup"><span data-stu-id="ac586-114">Binary</span></span>| <span data-ttu-id="ac586-115">Identificador de chave personalizada</span><span class="sxs-lookup"><span data-stu-id="ac586-115">Custom key identifier</span></span> |
|<span data-ttu-id="ac586-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ac586-116">endDateTime</span></span>|<span data-ttu-id="ac586-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac586-117">DateTimeOffset</span></span>|<span data-ttu-id="ac586-118">A data e a hora em que a credencial expira. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ac586-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac586-119">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ac586-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ac586-120">keyId</span><span class="sxs-lookup"><span data-stu-id="ac586-120">keyId</span></span>|<span data-ttu-id="ac586-121">Guid</span><span class="sxs-lookup"><span data-stu-id="ac586-121">Guid</span></span>|<span data-ttu-id="ac586-122">O identificador exclusivo (GUID) da chave.</span><span class="sxs-lookup"><span data-stu-id="ac586-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="ac586-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ac586-123">startDateTime</span></span>|<span data-ttu-id="ac586-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ac586-124">DateTimeOffset</span></span>|<span data-ttu-id="ac586-125">A data e a hora em que a credencial se torna válida. O tipo TIMESTAMP representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="ac586-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ac586-126">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ac586-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ac586-127">type</span><span class="sxs-lookup"><span data-stu-id="ac586-127">type</span></span>|<span data-ttu-id="ac586-128">String</span><span class="sxs-lookup"><span data-stu-id="ac586-128">String</span></span>|<span data-ttu-id="ac586-129">O tipo de credencial de chave; por exemplo, "simétrico".</span><span class="sxs-lookup"><span data-stu-id="ac586-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="ac586-130">ocorrência</span><span class="sxs-lookup"><span data-stu-id="ac586-130">usage</span></span>|<span data-ttu-id="ac586-131">String</span><span class="sxs-lookup"><span data-stu-id="ac586-131">String</span></span>|<span data-ttu-id="ac586-132">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; por exemplo, "Verify".</span><span class="sxs-lookup"><span data-stu-id="ac586-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="ac586-133">chave</span><span class="sxs-lookup"><span data-stu-id="ac586-133">key</span></span>|<span data-ttu-id="ac586-134">Binário</span><span class="sxs-lookup"><span data-stu-id="ac586-134">Binary</span></span>|            |

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
