---
title: tipo de recurso de keyCredential
description: Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço. A propriedade **keyCredentials** das entidades que aplicativo e servicePrincipal é uma coleção de **keyCredential**.
ms.openlocfilehash: d4509360c0425c255566b9f77b9ecd96cf349dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033458"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="34522-104">tipo de recurso de keyCredential</span><span class="sxs-lookup"><span data-stu-id="34522-104">keyCredential resource type</span></span>

> <span data-ttu-id="34522-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="34522-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="34522-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="34522-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="34522-107">Contém uma credencial de chave associada a um aplicativo ou uma entidade de serviço.</span><span class="sxs-lookup"><span data-stu-id="34522-107">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="34522-108">A propriedade **keyCredentials** das entidades que [aplicativo](application.md) e [servicePrincipal](serviceprincipal.md) é uma coleção de **keyCredential**.</span><span class="sxs-lookup"><span data-stu-id="34522-108">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="34522-109">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34522-109">JSON representation</span></span>

<span data-ttu-id="34522-110">Veja a seguir uma representação JSON do recurso</span><span class="sxs-lookup"><span data-stu-id="34522-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="34522-111">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34522-111">Properties</span></span>
| <span data-ttu-id="34522-112">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34522-112">Property</span></span>     | <span data-ttu-id="34522-113">Tipo</span><span class="sxs-lookup"><span data-stu-id="34522-113">Type</span></span>   |<span data-ttu-id="34522-114">Descrição</span><span class="sxs-lookup"><span data-stu-id="34522-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="34522-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="34522-115">customKeyIdentifier</span></span>|<span data-ttu-id="34522-116">Binário</span><span class="sxs-lookup"><span data-stu-id="34522-116">Binary</span></span>| <span data-ttu-id="34522-117">Identificador de chave personalizado</span><span class="sxs-lookup"><span data-stu-id="34522-117">Custom key identifier</span></span> |
|<span data-ttu-id="34522-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="34522-118">endDateTime</span></span>|<span data-ttu-id="34522-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34522-119">DateTimeOffset</span></span>|<span data-ttu-id="34522-120">A data e hora em que a credencial de expiração. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="34522-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34522-121">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="34522-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="34522-122">keyId</span><span class="sxs-lookup"><span data-stu-id="34522-122">keyId</span></span>|<span data-ttu-id="34522-123">Guid</span><span class="sxs-lookup"><span data-stu-id="34522-123">Guid</span></span>|<span data-ttu-id="34522-124">O identificador exclusivo (GUID) para a chave.</span><span class="sxs-lookup"><span data-stu-id="34522-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="34522-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="34522-125">startDateTime</span></span>|<span data-ttu-id="34522-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34522-126">DateTimeOffset</span></span>|<span data-ttu-id="34522-127">A data e hora em que a credencial torna-se válido. O tipo de carimbo de hora representa as informações de data e hora usando o formato ISO 8601 e é sempre em horário UTC.</span><span class="sxs-lookup"><span data-stu-id="34522-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34522-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="34522-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="34522-129">type</span><span class="sxs-lookup"><span data-stu-id="34522-129">type</span></span>|<span data-ttu-id="34522-130">String</span><span class="sxs-lookup"><span data-stu-id="34522-130">String</span></span>|<span data-ttu-id="34522-131">O tipo de credencial de chave; Por exemplo, "Simétrico".</span><span class="sxs-lookup"><span data-stu-id="34522-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="34522-132">uso</span><span class="sxs-lookup"><span data-stu-id="34522-132">usage</span></span>|<span data-ttu-id="34522-133">String</span><span class="sxs-lookup"><span data-stu-id="34522-133">String</span></span>|<span data-ttu-id="34522-134">Uma cadeia de caracteres que descreve a finalidade para a qual a chave pode ser usada; Por exemplo, "Verificar".</span><span class="sxs-lookup"><span data-stu-id="34522-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="34522-135">chave</span><span class="sxs-lookup"><span data-stu-id="34522-135">key</span></span>|<span data-ttu-id="34522-136">Binário</span><span class="sxs-lookup"><span data-stu-id="34522-136">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->