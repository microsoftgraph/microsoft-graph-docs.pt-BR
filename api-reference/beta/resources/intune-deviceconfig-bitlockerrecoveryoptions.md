---
title: tipo de recurso de bitLockerRecoveryOptions
description: Opções de recuperação do BitLocker.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df1a2d0a9be3f4ec52b5fa289d0315bda36e4a59
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398510"
---
# <a name="bitlockerrecoveryoptions-resource-type"></a><span data-ttu-id="c9d2a-103">tipo de recurso de bitLockerRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="c9d2a-103">bitLockerRecoveryOptions resource type</span></span>

> <span data-ttu-id="c9d2a-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="c9d2a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c9d2a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9d2a-107">Opções de recuperação do BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-107">BitLocker Recovery Options.</span></span>

## <a name="properties"></a><span data-ttu-id="c9d2a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c9d2a-108">Properties</span></span>
|<span data-ttu-id="c9d2a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c9d2a-109">Property</span></span>|<span data-ttu-id="c9d2a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c9d2a-110">Type</span></span>|<span data-ttu-id="c9d2a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c9d2a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c9d2a-112">blockDataRecoveryAgent</span><span class="sxs-lookup"><span data-stu-id="c9d2a-112">blockDataRecoveryAgent</span></span>|<span data-ttu-id="c9d2a-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d2a-113">Boolean</span></span>|<span data-ttu-id="c9d2a-114">Indica se o bloqueio de agente de recuperação de dados baseada em certificado.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-114">Indicates whether to block certificate-based data recovery agent.</span></span>|
|<span data-ttu-id="c9d2a-115">recoveryPasswordUsage</span><span class="sxs-lookup"><span data-stu-id="c9d2a-115">recoveryPasswordUsage</span></span>|[<span data-ttu-id="c9d2a-116">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c9d2a-116">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c9d2a-117">Indica se os usuários são permitidos ou necessárias para gerar uma senha de recuperação de 48 dígitos para fixo ou disco do sistema.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-117">Indicates whether users are allowed or required to generate a 48-digit recovery password for fixed or system disk.</span></span> <span data-ttu-id="c9d2a-118">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-118">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c9d2a-119">recoveryKeyUsage</span><span class="sxs-lookup"><span data-stu-id="c9d2a-119">recoveryKeyUsage</span></span>|[<span data-ttu-id="c9d2a-120">configurationUsage</span><span class="sxs-lookup"><span data-stu-id="c9d2a-120">configurationUsage</span></span>](../resources/intune-deviceconfig-configurationusage.md)|<span data-ttu-id="c9d2a-121">Indica se os usuários são permitidos ou necessárias para gerar uma chave de recuperação de 256 bits para fixo ou disco do sistema.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-121">Indicates whether users are allowed or required to generate a 256-bit recovery key for fixed or system disk.</span></span> <span data-ttu-id="c9d2a-122">Os valores possíveis são: `blocked`, `required`, `allowed`.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-122">Possible values are: `blocked`, `required`, `allowed`.</span></span>|
|<span data-ttu-id="c9d2a-123">hideRecoveryOptions</span><span class="sxs-lookup"><span data-stu-id="c9d2a-123">hideRecoveryOptions</span></span>|<span data-ttu-id="c9d2a-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d2a-124">Boolean</span></span>|<span data-ttu-id="c9d2a-125">Indica se deve ou não permitidas mostrando as opções de recuperação no Assistente de configuração de disco BitLocker para fixo ou disco do sistema.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-125">Indicates whether or not to allow showing recovery options in BitLocker Setup Wizard for fixed or system disk.</span></span>|
|<span data-ttu-id="c9d2a-126">enableRecoveryInformationSaveToStore</span><span class="sxs-lookup"><span data-stu-id="c9d2a-126">enableRecoveryInformationSaveToStore</span></span>|<span data-ttu-id="c9d2a-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d2a-127">Boolean</span></span>|<span data-ttu-id="c9d2a-128">Indica se deve ou não permitir que as informações de recuperação BitLocker armazenar no AD DS.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-128">Indicates whether or not to allow BitLocker recovery information to store in AD DS.</span></span>|
|<span data-ttu-id="c9d2a-129">recoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="c9d2a-129">recoveryInformationToStore</span></span>|[<span data-ttu-id="c9d2a-130">bitLockerRecoveryInformationType</span><span class="sxs-lookup"><span data-stu-id="c9d2a-130">bitLockerRecoveryInformationType</span></span>](../resources/intune-deviceconfig-bitlockerrecoveryinformationtype.md)|<span data-ttu-id="c9d2a-131">Configure quais partes de informações de recuperação do BitLocker são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-131">Configure what pieces of BitLocker recovery information are stored to AD DS.</span></span> <span data-ttu-id="c9d2a-132">Os valores possíveis são: `passwordAndKey` e `passwordOnly`.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-132">Possible values are: `passwordAndKey`, `passwordOnly`.</span></span>|
|<span data-ttu-id="c9d2a-133">enableBitLockerAfterRecoveryInformationToStore</span><span class="sxs-lookup"><span data-stu-id="c9d2a-133">enableBitLockerAfterRecoveryInformationToStore</span></span>|<span data-ttu-id="c9d2a-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="c9d2a-134">Boolean</span></span>|<span data-ttu-id="c9d2a-135">Indica se deseja ou não habilitar o BitLocker até que as informações de recuperação são armazenadas no AD DS.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-135">Indicates whether or not to enable BitLocker until recovery information is stored in AD DS.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c9d2a-136">Relações</span><span class="sxs-lookup"><span data-stu-id="c9d2a-136">Relationships</span></span>
<span data-ttu-id="c9d2a-137">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c9d2a-137">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c9d2a-138">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c9d2a-138">JSON Representation</span></span>
<span data-ttu-id="c9d2a-139">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c9d2a-139">Here is a JSON representation of the resource.</span></span>
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




