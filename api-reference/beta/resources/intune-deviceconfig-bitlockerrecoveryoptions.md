---
title: tipo de recurso bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 0c77cb413202ce713ce658da633f351f07286a03
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42527032"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="8cff4-103">tipo de recurso bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="8cff4-103">bitLockerRecoveryOptions resource type</span></span>

<span data-ttu-id="8cff4-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="8cff4-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="8cff4-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="8cff4-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8cff4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="8cff4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8cff4-107">Opções de recuperação do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8cff4-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="8cff4-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8cff4-108">Properties</span></span>
|<span data-ttu-id="8cff4-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8cff4-109">Property</span></span>|<span data-ttu-id="8cff4-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8cff4-110">Type</span></span>|<span data-ttu-id="8cff4-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8cff4-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8cff4-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="8cff4-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="8cff4-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cff4-113">Boolean</span></span>|<span data-ttu-id="8cff4-114">Indica se o agente de recuperação de dados baseado em certificado deve ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="8cff4-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="8cff4-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="8cff4-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="8cff4-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="8cff4-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="8cff4-117">Indica se os usuários são permitidos ou necessários para gerar uma senha de recuperação de 48 dígitos para o disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="8cff4-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="8cff4-118">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="8cff4-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="8cff4-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="8cff4-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="8cff4-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="8cff4-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="8cff4-121">Indica se os usuários são permitidos ou necessários para gerar uma chave de recuperação de 256 bits para o disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="8cff4-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="8cff4-122">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="8cff4-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="8cff4-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="8cff4-123">hideRecoveryOptions</span></span>|<span data-ttu-id="8cff4-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cff4-124">Boolean</span></span>|<span data-ttu-id="8cff4-125">Indica se a exibição das opções de recuperação no assistente de configuração do BitLocker deve ou não ser permitida no disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="8cff4-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="8cff4-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="8cff4-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="8cff4-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cff4-127">Boolean</span></span>|<span data-ttu-id="8cff4-128">Indica se as informações de recuperação do BitLocker devem ou não ser armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="8cff4-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="8cff4-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="8cff4-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="8cff4-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="8cff4-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="8cff4-131">Configure quais partes das informações de recuperação do BitLocker são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="8cff4-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="8cff4-132">Os valores possíveis são: `passwordAndKey` e `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="8cff4-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="8cff4-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="8cff4-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="8cff4-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="8cff4-134">Boolean</span></span>|<span data-ttu-id="8cff4-135">Indica se o BitLocker deve ou não ser habilitado até que as informações de recuperação sejam armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="8cff4-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8cff4-136">Relações</span><span class="sxs-lookup"><span data-stu-id="8cff4-136">Relationships</span></span>
<span data-ttu-id="8cff4-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8cff4-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="8cff4-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8cff4-138">JSON Representation</span></span>
<span data-ttu-id="8cff4-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8cff4-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.bitLockerRecoveryOptions"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.bitLockerRecoveryOptions",
  "blockDataRecoveryAgent": true,
  "recoveryPasswordUsage": "String",
  "recoveryKeyUsage": "String",
  "hideRecoveryOptions": true,
  "enableRecoveryInformationSaveToStore": true,
  "recoveryInformationToStore": "String",
  "enableBitLockerAfterRecoveryInformationToStore": true
}
```



