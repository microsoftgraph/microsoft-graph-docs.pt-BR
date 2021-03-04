---
title: Tipo de recurso bitlockerRecoveryKey
description: Recurso de chave de recuperação do BitLocker
author: hafowler
localization_priority: Normal
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 466a5d907b3deb589ec1b70351903e24aba0ab32
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443150"
---
# <a name="bitlockerrecoverykey-resource-type"></a><span data-ttu-id="85456-103">Tipo de recurso bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="85456-103">bitlockerRecoveryKey resource type</span></span>

<span data-ttu-id="85456-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="85456-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="85456-105">Representa uma chave BitLocker armazenada que contém a chave de recuperação real por meio da **propriedade key.**</span><span class="sxs-lookup"><span data-stu-id="85456-105">Represents a stored BitLocker key that contains the actual recovery key via the **key** property.</span></span>

## <a name="methods"></a><span data-ttu-id="85456-106">Methods</span><span class="sxs-lookup"><span data-stu-id="85456-106">Methods</span></span>
|<span data-ttu-id="85456-107">Método</span><span class="sxs-lookup"><span data-stu-id="85456-107">Method</span></span>|<span data-ttu-id="85456-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="85456-108">Return type</span></span>|<span data-ttu-id="85456-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="85456-109">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="85456-110">Listar recoveryKeys</span><span class="sxs-lookup"><span data-stu-id="85456-110">List recoveryKeys</span></span>](../api/bitlocker-list-recoverykeys.md)|<span data-ttu-id="85456-111">[Coleção bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="85456-111">[bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) collection</span></span>|<span data-ttu-id="85456-112">Obter uma lista dos [objetos bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) e suas propriedades.</span><span class="sxs-lookup"><span data-stu-id="85456-112">Get a list of the [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) objects and their properties.</span></span>|
|[<span data-ttu-id="85456-113">Obter bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="85456-113">Get bitlockerRecoveryKey</span></span>](../api/bitlockerrecoverykey-get.md)|[<span data-ttu-id="85456-114">bitlockerRecoveryKey</span><span class="sxs-lookup"><span data-stu-id="85456-114">bitlockerRecoveryKey</span></span>](../resources/bitlockerrecoverykey.md)|<span data-ttu-id="85456-115">Recupere as propriedades e as relações de um [objeto bitlockerRecoveryKey.](../resources/bitlockerrecoverykey.md)</span><span class="sxs-lookup"><span data-stu-id="85456-115">Retrieve the properties and relationships of a [bitlockerRecoveryKey](../resources/bitlockerrecoverykey.md) object.</span></span> <span data-ttu-id="85456-116">Observação: a **propriedade key** não é retornada por padrão.</span><span class="sxs-lookup"><span data-stu-id="85456-116">Note: The **key** property is not returned by default.</span></span>|

> <span data-ttu-id="85456-117">**Observação**: apenas algumas funções têm as permissões para chamar essas APIs.</span><span class="sxs-lookup"><span data-stu-id="85456-117">**Note**: Only some roles have the permissions to call these APIs.</span></span>

## <a name="properties"></a><span data-ttu-id="85456-118">Propriedades</span><span class="sxs-lookup"><span data-stu-id="85456-118">Properties</span></span>
|<span data-ttu-id="85456-119">Propriedade</span><span class="sxs-lookup"><span data-stu-id="85456-119">Property</span></span>|<span data-ttu-id="85456-120">Tipo</span><span class="sxs-lookup"><span data-stu-id="85456-120">Type</span></span>|<span data-ttu-id="85456-121">Descrição</span><span class="sxs-lookup"><span data-stu-id="85456-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="85456-122">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="85456-122">createdDateTime</span></span>|<span data-ttu-id="85456-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="85456-123">DateTimeOffset</span></span>|<span data-ttu-id="85456-124">A data e a hora em que a chave foi originalmente respaldada no Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="85456-124">The date and time when the key was originally backed up to Azure Active Directory.</span></span>|
|<span data-ttu-id="85456-125">deviceId</span><span class="sxs-lookup"><span data-stu-id="85456-125">deviceId</span></span>|<span data-ttu-id="85456-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="85456-126">String</span></span>|<span data-ttu-id="85456-127">ID do dispositivo de onde a chave BitLocker é originalmente respaldada.</span><span class="sxs-lookup"><span data-stu-id="85456-127">ID of the device the BitLocker key is originally backed up from.</span></span>|
|<span data-ttu-id="85456-128">id</span><span class="sxs-lookup"><span data-stu-id="85456-128">id</span></span>|<span data-ttu-id="85456-129">String</span><span class="sxs-lookup"><span data-stu-id="85456-129">String</span></span>|<span data-ttu-id="85456-130">O identificador exclusivo da chave BitLocker.</span><span class="sxs-lookup"><span data-stu-id="85456-130">The unique identifier for the BitLocker key.</span></span>|
|<span data-ttu-id="85456-131">chave</span><span class="sxs-lookup"><span data-stu-id="85456-131">key</span></span>|<span data-ttu-id="85456-132">String</span><span class="sxs-lookup"><span data-stu-id="85456-132">String</span></span>|<span data-ttu-id="85456-133">A chave de recuperação BitLocker.</span><span class="sxs-lookup"><span data-stu-id="85456-133">The BitLocker recovery key.</span></span>|
|<span data-ttu-id="85456-134">volumeType</span><span class="sxs-lookup"><span data-stu-id="85456-134">volumeType</span></span>|<span data-ttu-id="85456-135">volumeType</span><span class="sxs-lookup"><span data-stu-id="85456-135">volumeType</span></span>|<span data-ttu-id="85456-136">Indica o tipo de volume ao qual a chave BitLocker está associada.</span><span class="sxs-lookup"><span data-stu-id="85456-136">Indicates the type of volume the BitLocker key is associated with.</span></span> <span data-ttu-id="85456-137">Os valores possíveis são: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span><span class="sxs-lookup"><span data-stu-id="85456-137">Possible values are: `operatingSystemVolume`, `fixedDataVolume`, `removableDataVolume`, `unknownFutureValue`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="85456-138">Relações</span><span class="sxs-lookup"><span data-stu-id="85456-138">Relationships</span></span>
<span data-ttu-id="85456-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="85456-139">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="85456-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="85456-140">JSON representation</span></span>
<span data-ttu-id="85456-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="85456-141">The following is a JSON representation of the resource.</span></span>
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

