---
title: tipo de recurso de logonUser
description: Contém informações com informações de estado sobre o usuário conectado nesse host
ms.openlocfilehash: 80ff69453e99f5cd5103f85cd7d8c45696057f7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27040122"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="a924d-103">tipo de recurso de logonUser</span><span class="sxs-lookup"><span data-stu-id="a924d-103">logonUser resource type</span></span>

<span data-ttu-id="a924d-104">Contém informações com informações de estado sobre o usuário conectado nesse host</span><span class="sxs-lookup"><span data-stu-id="a924d-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="a924d-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a924d-105">Properties</span></span>

| <span data-ttu-id="a924d-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a924d-106">Property</span></span>   | <span data-ttu-id="a924d-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="a924d-107">Type</span></span> |<span data-ttu-id="a924d-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="a924d-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a924d-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="a924d-109">accountDomain</span></span>|<span data-ttu-id="a924d-110">String</span><span class="sxs-lookup"><span data-stu-id="a924d-110">String</span></span>|<span data-ttu-id="a924d-111">Domínio da conta de usuário usada para logon.</span><span class="sxs-lookup"><span data-stu-id="a924d-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="a924d-112">accountName</span><span class="sxs-lookup"><span data-stu-id="a924d-112">accountName</span></span>|<span data-ttu-id="a924d-113">String</span><span class="sxs-lookup"><span data-stu-id="a924d-113">String</span></span>|<span data-ttu-id="a924d-114">Nome da conta da conta de usuário usada para logon.</span><span class="sxs-lookup"><span data-stu-id="a924d-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="a924d-115">accountType</span><span class="sxs-lookup"><span data-stu-id="a924d-115">accountType</span></span>|<span data-ttu-id="a924d-116">String</span><span class="sxs-lookup"><span data-stu-id="a924d-116">String</span></span>|<span data-ttu-id="a924d-117">Tipo de conta de usuário, por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="a924d-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="a924d-118">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="a924d-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="a924d-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="a924d-119">firstSeenDateTime</span></span>|<span data-ttu-id="a924d-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a924d-120">DateTimeOffset</span></span>|<span data-ttu-id="a924d-121">Data e hora em que o logon mais antigo por esta conta de usuário ocorreu (período determinado pelo provedor).</span><span class="sxs-lookup"><span data-stu-id="a924d-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="a924d-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a924d-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a924d-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a924d-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a924d-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="a924d-124">lastSeenDateTime</span></span>|<span data-ttu-id="a924d-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a924d-125">DateTimeOffset</span></span>|<span data-ttu-id="a924d-126">Data e hora em que o logon mais recente por esta conta de usuário ocorreu.</span><span class="sxs-lookup"><span data-stu-id="a924d-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="a924d-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a924d-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a924d-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="a924d-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="a924d-129">identificação de logon</span><span class="sxs-lookup"><span data-stu-id="a924d-129">logonId</span></span>|<span data-ttu-id="a924d-130">String</span><span class="sxs-lookup"><span data-stu-id="a924d-130">String</span></span>|<span data-ttu-id="a924d-131">ID de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="a924d-131">User logon ID.</span></span>|
|<span data-ttu-id="a924d-132">logonTypes</span><span class="sxs-lookup"><span data-stu-id="a924d-132">logonTypes</span></span>|<span data-ttu-id="a924d-133">String collection</span><span class="sxs-lookup"><span data-stu-id="a924d-133">String collection</span></span>|<span data-ttu-id="a924d-134">Coleção dos tipos de logon observados para o usuário conectado ao primeiro ao último vistas.</span><span class="sxs-lookup"><span data-stu-id="a924d-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="a924d-135">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="a924d-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a924d-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a924d-136">JSON representation</span></span>

<span data-ttu-id="a924d-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a924d-137">The following is a JSON representation of the resource.</span></span>

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