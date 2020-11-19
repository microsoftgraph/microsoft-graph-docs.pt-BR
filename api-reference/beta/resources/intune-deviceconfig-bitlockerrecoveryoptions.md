---
title: tipo de recurso bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: e381b559c291a3da86b7ee6f9a70a67dedf63bb7
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49260618"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="aefa9-103">tipo de recurso bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="aefa9-103">bitLockerRecoveryOptions resource type</span></span>

<span data-ttu-id="aefa9-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="aefa9-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="aefa9-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="aefa9-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="aefa9-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="aefa9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aefa9-107">Opções de recuperação do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="aefa9-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="aefa9-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="aefa9-108">Properties</span></span>
|<span data-ttu-id="aefa9-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="aefa9-109">Property</span></span>|<span data-ttu-id="aefa9-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="aefa9-110">Type</span></span>|<span data-ttu-id="aefa9-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="aefa9-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="aefa9-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="aefa9-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="aefa9-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="aefa9-113">Boolean</span></span>|<span data-ttu-id="aefa9-114">Indica se o agente de recuperação de dados baseado em certificado deve ser bloqueado.</span><span class="sxs-lookup"><span data-stu-id="aefa9-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="aefa9-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="aefa9-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="aefa9-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="aefa9-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="aefa9-117">Indica se os usuários são permitidos ou necessários para gerar uma senha de recuperação de 48 dígitos para o disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="aefa9-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="aefa9-118">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="aefa9-118">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="aefa9-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="aefa9-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="aefa9-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="aefa9-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="aefa9-121">Indica se os usuários são permitidos ou necessários para gerar uma chave de recuperação de 256 bits para o disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="aefa9-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="aefa9-122">Os valores possíveis são: `blocked`, `required`, `allowed`, `notConfigured`.</span><span class="sxs-lookup"><span data-stu-id="aefa9-122">Possible values are: `blocked`, `required`, `allowed`, `notConfigured`.</span></span>|
|<span data-ttu-id="aefa9-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="aefa9-123">hideRecoveryOptions</span></span>|<span data-ttu-id="aefa9-124">Booliano</span><span class="sxs-lookup"><span data-stu-id="aefa9-124">Boolean</span></span>|<span data-ttu-id="aefa9-125">Indica se a exibição das opções de recuperação no assistente de configuração do BitLocker deve ou não ser permitida no disco fixo ou do sistema.</span><span class="sxs-lookup"><span data-stu-id="aefa9-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="aefa9-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="aefa9-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="aefa9-127">Booliano</span><span class="sxs-lookup"><span data-stu-id="aefa9-127">Boolean</span></span>|<span data-ttu-id="aefa9-128">Indica se as informações de recuperação do BitLocker devem ou não ser armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="aefa9-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="aefa9-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="aefa9-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="aefa9-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="aefa9-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="aefa9-131">Configure quais partes das informações de recuperação do BitLocker são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="aefa9-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="aefa9-132">Os valores possíveis são: `passwordAndKey` e `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="aefa9-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="aefa9-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="aefa9-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="aefa9-134">Booliano</span><span class="sxs-lookup"><span data-stu-id="aefa9-134">Boolean</span></span>|<span data-ttu-id="aefa9-135">Indica se o BitLocker deve ou não ser habilitado até que as informações de recuperação sejam armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="aefa9-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="aefa9-136">Relações</span><span class="sxs-lookup"><span data-stu-id="aefa9-136">Relationships</span></span>
<span data-ttu-id="aefa9-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="aefa9-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="aefa9-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="aefa9-138">JSON Representation</span></span>
<span data-ttu-id="aefa9-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="aefa9-139">Here is a JSON representation of the resource.</span></span>
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




