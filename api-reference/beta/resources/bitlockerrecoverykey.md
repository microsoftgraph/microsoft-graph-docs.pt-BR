---
title: tipo de recurso bitlockerRecoveryKey
description: Recurso de chave de recuperação do BitLocker
author: hafowler
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 038feb77f7ca57d426a44c04b3d9c93ae29e5aa4
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48081943"
---
# <a name="bitlockerrecoverykey-resource-type"></a><span data-ttu-id="52142-103">tipo de recurso bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="52142-103">bitlockerRecoveryKey resource type</span></span>

<span data-ttu-id="52142-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="52142-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52142-105">Representa uma chave BitLocker armazenada que contém a chave de recuperação real por meio da propriedade **Key** .</span><span class="sxs-lookup"><span data-stu-id="52142-105">Represents a stored BitLocker key that contains the actual recovery key via the **key** property.</span></span>

## <a name="methods"></a><span data-ttu-id="52142-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="52142-106">Methods</span></span>
|<span data-ttu-id="52142-107">Método</span><span class="sxs-lookup"><span data-stu-id="52142-107">Method</span></span>|<span data-ttu-id="52142-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="52142-108">Return type</span></span>|<span data-ttu-id="52142-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="52142-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="52142-110">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="52142-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="52142-111">coleção [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="52142-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="52142-112">Obtenha uma lista dos objetos [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="52142-112">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span>|
|[<span data-ttu-id="52142-113">Obter bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="52142-113">Get bitlockerRecoveryKey</span></span>](../api/bitlockerrecoverykey-get.md)|[<span data-ttu-id="52142-114">bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="52142-114">bitlockerRecoveryKey</span></span>](../resources/bitlockerrecoverykey.md)|<span data-ttu-id="52142-115">Recupere as propriedades e os relacionamentos de um objeto [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) .</span><span class="sxs-lookup"><span data-stu-id="52142-115">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> <span data-ttu-id="52142-116">Observação: a propriedade **Key** não é retornada por padrão.</span><span class="sxs-lookup"><span data-stu-id="52142-116">Note: The **key** property is not returned by default.</span></span>|

> <span data-ttu-id="52142-117">**Observação**: apenas algumas funções têm as permissões para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="52142-117">**Note**: Only some roles have the permissions to call these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="52142-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="52142-118">Properties</span></span>
|<span data-ttu-id="52142-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="52142-119">Property</span></span>|<span data-ttu-id="52142-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="52142-120">Type</span></span>|<span data-ttu-id="52142-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="52142-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="52142-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="52142-122">createdDateTime</span></span>|<span data-ttu-id="52142-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="52142-123">DateTimeOffset</span></span>|<span data-ttu-id="52142-124">A data e a hora em que a chave foi originalmente convertida no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="52142-124">The date and time when the key was originally backed up to Azure Active Directory.</span></span>|
|<span data-ttu-id="52142-125">deviceId</span><span class="sxs-lookup"><span data-stu-id="52142-125">deviceId</span></span>|<span data-ttu-id="52142-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52142-126">String</span></span>|<span data-ttu-id="52142-127">ID do dispositivo do qual é feito o backup da chave BitLocker originalmente.</span><span class="sxs-lookup"><span data-stu-id="52142-127">ID of the device the BitLocker key is originally backed up from.</span></span>|
|<span data-ttu-id="52142-128">id</span><span class="sxs-lookup"><span data-stu-id="52142-128">id</span></span>|<span data-ttu-id="52142-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52142-129">String</span></span>|<span data-ttu-id="52142-130">O identificador exclusivo da chave do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="52142-130">The unique identifier for the BitLocker key.</span></span>|
|<span data-ttu-id="52142-131">chave</span><span class="sxs-lookup"><span data-stu-id="52142-131">key</span></span>|<span data-ttu-id="52142-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="52142-132">String</span></span>|<span data-ttu-id="52142-133">A chave de recuperação do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="52142-133">The BitLocker recovery key.</span></span>|
|<span data-ttu-id="52142-134">volumetype</span><span class="sxs-lookup"><span data-stu-id="52142-134">volumeType</span></span>|<span data-ttu-id="52142-135">volumetype</span><span class="sxs-lookup"><span data-stu-id="52142-135">volumeType</span></span>|<span data-ttu-id="52142-136">Indica o tipo de volume ao qual a chave BitLocker está associada.</span><span class="sxs-lookup"><span data-stu-id="52142-136">Indicates the type of volume the BitLocker key is associated with.</span></span> <span data-ttu-id="52142-137">Os valores possíveis são: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="52142-137">Possible values are: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="52142-138">Relações</span><span class="sxs-lookup"><span data-stu-id="52142-138">Relationships</span></span>
<span data-ttu-id="52142-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="52142-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52142-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="52142-140">JSON representation</span></span>
<span data-ttu-id="52142-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="52142-141">The following is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.bitlockerRecoveryKey",
  "baseType": "microsoft.graph.entity",
  "openType": false
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitlockerRecoveryKey",
  "id": "b465e4e8-e4e8-b465-e8e4-65b4e8e465b4",
  "createdDateTime": "2020-06-15T13:45:30.0000000Z",
  "volumeType": 1,
  "deviceId": "1ab40ab2-32a8-4b00-b6b5-ba724e407de9",
  "key": "123456-231453-873456-213546-654678-765689-123456-324565"
}
```

