---
title: tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 08053b2e3ba42c167edebb3678b41ccb3531e078
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009913"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="b07a1-103">tipo de recurso logonUser</span><span class="sxs-lookup"><span data-stu-id="b07a1-103">logonUser resource type</span></span>

<span data-ttu-id="b07a1-104">Contém informações de estado sobre o usuário conectado neste host</span><span class="sxs-lookup"><span data-stu-id="b07a1-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="b07a1-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b07a1-105">Properties</span></span>

| <span data-ttu-id="b07a1-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b07a1-106">Property</span></span>   | <span data-ttu-id="b07a1-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b07a1-107">Type</span></span> |<span data-ttu-id="b07a1-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b07a1-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b07a1-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="b07a1-109">accountDomain</span></span>|<span data-ttu-id="b07a1-110">String</span><span class="sxs-lookup"><span data-stu-id="b07a1-110">String</span></span>|<span data-ttu-id="b07a1-111">Domínio da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="b07a1-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="b07a1-112">accountName</span><span class="sxs-lookup"><span data-stu-id="b07a1-112">accountName</span></span>|<span data-ttu-id="b07a1-113">String</span><span class="sxs-lookup"><span data-stu-id="b07a1-113">String</span></span>|<span data-ttu-id="b07a1-114">Nome da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="b07a1-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="b07a1-115">accountType</span><span class="sxs-lookup"><span data-stu-id="b07a1-115">accountType</span></span>|<span data-ttu-id="b07a1-116">String</span><span class="sxs-lookup"><span data-stu-id="b07a1-116">String</span></span>|<span data-ttu-id="b07a1-117">Tipo de conta de usuário, por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="b07a1-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="b07a1-118">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="b07a1-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="b07a1-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="b07a1-119">firstSeenDateTime</span></span>|<span data-ttu-id="b07a1-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b07a1-120">DateTimeOffset</span></span>|<span data-ttu-id="b07a1-121">Data e hora em que o logon mais antigo por essa conta de usuário ocorreu (período determinado pelo provedor).</span><span class="sxs-lookup"><span data-stu-id="b07a1-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="b07a1-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b07a1-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b07a1-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b07a1-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b07a1-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="b07a1-124">lastSeenDateTime</span></span>|<span data-ttu-id="b07a1-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b07a1-125">DateTimeOffset</span></span>|<span data-ttu-id="b07a1-126">DateTime no qual a conta de usuário tem o logon mais recente.</span><span class="sxs-lookup"><span data-stu-id="b07a1-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="b07a1-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="b07a1-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b07a1-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="b07a1-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="b07a1-129">LogonId</span><span class="sxs-lookup"><span data-stu-id="b07a1-129">logonId</span></span>|<span data-ttu-id="b07a1-130">String</span><span class="sxs-lookup"><span data-stu-id="b07a1-130">String</span></span>|<span data-ttu-id="b07a1-131">ID de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="b07a1-131">User logon ID.</span></span>|
|<span data-ttu-id="b07a1-132">Logontypesowner</span><span class="sxs-lookup"><span data-stu-id="b07a1-132">logonTypes</span></span>|<span data-ttu-id="b07a1-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="b07a1-133">String collection</span></span>|<span data-ttu-id="b07a1-134">Coleção dos tipos de logon observados para o usuário conectado da primeira vez para a última vista.</span><span class="sxs-lookup"><span data-stu-id="b07a1-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="b07a1-135">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="b07a1-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b07a1-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b07a1-136">JSON representation</span></span>

<span data-ttu-id="b07a1-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b07a1-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.logonUser"
}-->

```json
{
  "accountDomain": "String",
  "accountName": "String",
  "accountType": "String",
  "firstSeenDateTime": "String (timestamp)",
  "lastSeenDateTime": "String (timestamp)",
  "logonId": "String",
  "logonTypes": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "logonUser resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
