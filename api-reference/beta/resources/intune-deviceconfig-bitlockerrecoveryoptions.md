---
title: tipo de recurso bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf88795ac9f2708bc03607bc5d48d5ec69a822eb
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34991048"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="cf730-103">tipo de recurso bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="cf730-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="cf730-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="cf730-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cf730-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cf730-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cf730-106">Opções de recuperação do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="cf730-106">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="cf730-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="cf730-107">Properties</span></span>
|<span data-ttu-id="cf730-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="cf730-108">Property</span></span>|<span data-ttu-id="cf730-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="cf730-109">Type</span></span>|<span data-ttu-id="cf730-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="cf730-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf730-111">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="cf730-111">blockDataRecoveryAgent</span></span>|<span data-ttu-id="cf730-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf730-112">Boolean</span></span>|<span data-ttu-id="cf730-113">Indica se o agente de recuperação de dados baseado em certificado deve ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="cf730-113">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="cf730-114">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="cf730-114">recoveryPasswordUsage</span></span>|[<span data-ttu-id="cf730-115">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="cf730-115">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="cf730-116">Indica se os usuários são permitidos ou necessários para gerar uma senha de recuperação de 48 dígitos para o disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="cf730-116">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="cf730-117">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cf730-117">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="cf730-118">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="cf730-118">recoveryKeyUsage</span></span>|[<span data-ttu-id="cf730-119">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="cf730-119">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="cf730-120">Indica se os usuários são permitidos ou necessários para gerar uma chave de recuperação de 256 bits para o disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="cf730-120">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="cf730-121">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="cf730-121">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="cf730-122">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="cf730-122">hideRecoveryOptions</span></span>|<span data-ttu-id="cf730-123">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf730-123">Boolean</span></span>|<span data-ttu-id="cf730-124">Indica se a exibição das opções de recuperação no assistente de configuração do BitLocker deve ou não ser permitida no disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="cf730-124">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="cf730-125">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="cf730-125">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="cf730-126">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf730-126">Boolean</span></span>|<span data-ttu-id="cf730-127">Indica se as informações de recuperação do BitLocker devem ou não ser armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="cf730-127">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="cf730-128">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="cf730-128">recoveryInformationToStore</span></span>|[<span data-ttu-id="cf730-129">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="cf730-129">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="cf730-130">Configure quais partes das informações de recuperação do BitLocker são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="cf730-130">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="cf730-131">Os valores possíveis são: `passwordAndKey` e `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="cf730-131">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="cf730-132">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="cf730-132">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="cf730-133">Booliano</span><span class="sxs-lookup"><span data-stu-id="cf730-133">Boolean</span></span>|<span data-ttu-id="cf730-134">Indica se o BitLocker deve ou não ser habilitado até que as informações de recuperação sejam armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="cf730-134">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cf730-135">Relações</span><span class="sxs-lookup"><span data-stu-id="cf730-135">Relationships</span></span>
<span data-ttu-id="cf730-136">Nenhum</span><span class="sxs-lookup"><span data-stu-id="cf730-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="cf730-137">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="cf730-137">JSON Representation</span></span>
<span data-ttu-id="cf730-138">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="cf730-138">Here is a JSON representation of the resource.</span></span>
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





