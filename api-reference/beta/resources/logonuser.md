---
title: tipo de recurso logonUser
description: Contém informações de estado sobre o usuário conectado neste host
localization_priority: Normal
ms.openlocfilehash: 3b7862555c62eb16aaceaa53d4df58541426e08a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562654"
---
# <a name="logonuser-resource-type"></a><span data-ttu-id="aaa1c-103">tipo de recurso logonUser</span><span class="sxs-lookup"><span data-stu-id="aaa1c-103">logonUser resource type</span></span>

<span data-ttu-id="aaa1c-104">Contém informações de estado sobre o usuário conectado neste host</span><span class="sxs-lookup"><span data-stu-id="aaa1c-104">Contains stateful information about the logged on user on this host</span></span>

## <a name="properties"></a><span data-ttu-id="aaa1c-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aaa1c-105">Properties</span></span>

| <span data-ttu-id="aaa1c-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aaa1c-106">Property</span></span>   | <span data-ttu-id="aaa1c-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="aaa1c-107">Type</span></span> |<span data-ttu-id="aaa1c-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="aaa1c-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aaa1c-109">accountDomain</span><span class="sxs-lookup"><span data-stu-id="aaa1c-109">accountDomain</span></span>|<span data-ttu-id="aaa1c-110">String</span><span class="sxs-lookup"><span data-stu-id="aaa1c-110">String</span></span>|<span data-ttu-id="aaa1c-111">Domínio da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-111">Domain of user account used to logon.</span></span>|
|<span data-ttu-id="aaa1c-112">accountName</span><span class="sxs-lookup"><span data-stu-id="aaa1c-112">accountName</span></span>|<span data-ttu-id="aaa1c-113">String</span><span class="sxs-lookup"><span data-stu-id="aaa1c-113">String</span></span>|<span data-ttu-id="aaa1c-114">Nome da conta de usuário usada para fazer logon.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-114">Account name of user account used to logon.</span></span>|
|<span data-ttu-id="aaa1c-115">accountType</span><span class="sxs-lookup"><span data-stu-id="aaa1c-115">accountType</span></span>|<span data-ttu-id="aaa1c-116">String</span><span class="sxs-lookup"><span data-stu-id="aaa1c-116">String</span></span>|<span data-ttu-id="aaa1c-117">Tipo de conta de usuário, por definição do Windows.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-117">User Account type, per Windows definition.</span></span> <span data-ttu-id="aaa1c-118">Os valores possíveis são: `unknown`, `standard`, `power`, `administrator`.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-118">Possible values are: `unknown`, `standard`, `power`, `administrator`.</span></span>|
|<span data-ttu-id="aaa1c-119">firstSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="aaa1c-119">firstSeenDateTime</span></span>|<span data-ttu-id="aaa1c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaa1c-120">DateTimeOffset</span></span>|<span data-ttu-id="aaa1c-121">Data e hora em que o logon mais antigo por essa conta de usuário ocorreu (período determinado pelo provedor).</span><span class="sxs-lookup"><span data-stu-id="aaa1c-121">DateTime at which the earliest logon by this user account occurred (provider-determined period).</span></span> <span data-ttu-id="aaa1c-122">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-122">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aaa1c-123">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aaa1c-124">lastSeenDateTime</span><span class="sxs-lookup"><span data-stu-id="aaa1c-124">lastSeenDateTime</span></span>|<span data-ttu-id="aaa1c-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aaa1c-125">DateTimeOffset</span></span>|<span data-ttu-id="aaa1c-126">DateTime no qual a conta de usuário tem o logon mais recente.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-126">DateTime at which the latest logon by this user account occurred.</span></span> <span data-ttu-id="aaa1c-127">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-127">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aaa1c-128">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span>|
|<span data-ttu-id="aaa1c-129">LogonId</span><span class="sxs-lookup"><span data-stu-id="aaa1c-129">logonId</span></span>|<span data-ttu-id="aaa1c-130">String</span><span class="sxs-lookup"><span data-stu-id="aaa1c-130">String</span></span>|<span data-ttu-id="aaa1c-131">ID de logon do usuário.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-131">User logon ID.</span></span>|
|<span data-ttu-id="aaa1c-132">Logontypesowner</span><span class="sxs-lookup"><span data-stu-id="aaa1c-132">logonTypes</span></span>|<span data-ttu-id="aaa1c-133">Coleção de cadeias de caracteres</span><span class="sxs-lookup"><span data-stu-id="aaa1c-133">String collection</span></span>|<span data-ttu-id="aaa1c-134">Coleção dos tipos de logon observados para o usuário conectado da primeira vez para a última vista.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-134">Collection of the logon types observed for the logged on user from when first to last seen.</span></span> <span data-ttu-id="aaa1c-135">Os possíveis valores são: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-135">Possible values are: `unknown`, `interactive`, `remoteInteractive`, `network`, `batch`, `service`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aaa1c-136">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aaa1c-136">JSON representation</span></span>

<span data-ttu-id="aaa1c-137">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aaa1c-137">The following is a JSON representation of the resource.</span></span>

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
