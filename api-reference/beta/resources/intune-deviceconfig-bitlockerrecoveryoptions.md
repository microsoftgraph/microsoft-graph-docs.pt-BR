---
title: tipo de recurso de bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
author: tfitzmac
ms.openlocfilehash: c85ce3111ed88ce8e8bf54c98d5fd3122571a0be
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27310602"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="4c15c-103">tipo de recurso de bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="4c15c-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="4c15c-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c15c-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4c15c-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c15c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c15c-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="4c15c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c15c-107">Opções de recuperação do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="4c15c-107">BitLocker Recovery Options.</span></span>
## <a name="properties"></a><span data-ttu-id="4c15c-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="4c15c-108">Properties</span></span>
|<span data-ttu-id="4c15c-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c15c-109">Property</span></span>|<span data-ttu-id="4c15c-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c15c-110">Type</span></span>|<span data-ttu-id="4c15c-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c15c-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c15c-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="4c15c-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="4c15c-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c15c-113">Boolean</span></span>|<span data-ttu-id="4c15c-114">Indica se o bloqueio de agente de recuperação de dados baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="4c15c-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="4c15c-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="4c15c-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="4c15c-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="4c15c-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4c15c-117">Indica se os usuários são permitidos ou necessárias para gerar uma senha de recuperação de 48 dígitos para fixo ou disco do sistema.</span><span class="sxs-lookup"><span data-stu-id="4c15c-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="4c15c-118">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4c15c-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4c15c-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="4c15c-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="4c15c-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="4c15c-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="4c15c-121">Indica se os usuários são permitidos ou necessárias para gerar uma chave de recuperação de 256 bits para fixo ou disco do sistema.</span><span class="sxs-lookup"><span data-stu-id="4c15c-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="4c15c-122">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="4c15c-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="4c15c-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="4c15c-123">hideRecoveryOptions</span></span>|<span data-ttu-id="4c15c-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c15c-124">Boolean</span></span>|<span data-ttu-id="4c15c-125">Indica se deve ou não permitidas mostrando as opções de recuperação no Assistente de configuração de disco BitLocker para fixo ou disco do sistema.</span><span class="sxs-lookup"><span data-stu-id="4c15c-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="4c15c-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="4c15c-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="4c15c-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c15c-127">Boolean</span></span>|<span data-ttu-id="4c15c-128">Indica se deve ou não permitir que as informações de recuperação BitLocker armazenar no AD DS.</span><span class="sxs-lookup"><span data-stu-id="4c15c-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="4c15c-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="4c15c-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="4c15c-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="4c15c-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="4c15c-131">Configure quais partes de informações de recuperação do BitLocker são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="4c15c-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="4c15c-132">Os valores possíveis são: `passwordAndKey` e `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="4c15c-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="4c15c-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="4c15c-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="4c15c-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c15c-134">Boolean</span></span>|<span data-ttu-id="4c15c-135">Indica se deseja ou não habilitar o BitLocker até que as informações de recuperação são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="4c15c-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4c15c-136">Relações</span><span class="sxs-lookup"><span data-stu-id="4c15c-136">Relationships</span></span>
<span data-ttu-id="4c15c-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="4c15c-137">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4c15c-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="4c15c-138">JSON Representation</span></span>
<span data-ttu-id="4c15c-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="4c15c-139">Here is a JSON representation of the resource.</span></span>
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





