---
title: Tipo de recurso deviceManagementConfigurationSettingInstanceTemplate
description: Modelo de instância de configuração
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 76d8c9b985a3ca30f0d2a0a4144128d0e7a1baff
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868325"
---
# <a name="devicemanagementconfigurationsettinginstancetemplate-resource-type"></a><span data-ttu-id="faa1a-103">Tipo de recurso deviceManagementConfigurationSettingInstanceTemplate</span><span class="sxs-lookup"><span data-stu-id="faa1a-103">deviceManagementConfigurationSettingInstanceTemplate resource type</span></span>

<span data-ttu-id="faa1a-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="faa1a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="faa1a-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="faa1a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="faa1a-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="faa1a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="faa1a-107">Modelo de instância de configuração</span><span class="sxs-lookup"><span data-stu-id="faa1a-107">Setting Instance Template</span></span>

## <a name="properties"></a><span data-ttu-id="faa1a-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="faa1a-108">Properties</span></span>
|<span data-ttu-id="faa1a-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="faa1a-109">Property</span></span>|<span data-ttu-id="faa1a-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="faa1a-110">Type</span></span>|<span data-ttu-id="faa1a-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="faa1a-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="faa1a-112">settingInstanceTemplateId</span><span class="sxs-lookup"><span data-stu-id="faa1a-112">settingInstanceTemplateId</span></span>|<span data-ttu-id="faa1a-113">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="faa1a-113">String</span></span>|<span data-ttu-id="faa1a-114">Id do modelo de instância de configuração</span><span class="sxs-lookup"><span data-stu-id="faa1a-114">Setting Instance Template Id</span></span>|
|<span data-ttu-id="faa1a-115">settingDefinitionId</span><span class="sxs-lookup"><span data-stu-id="faa1a-115">settingDefinitionId</span></span>|<span data-ttu-id="faa1a-116">Cadeia de Caracteres</span><span class="sxs-lookup"><span data-stu-id="faa1a-116">String</span></span>|<span data-ttu-id="faa1a-117">Definindo id de definição</span><span class="sxs-lookup"><span data-stu-id="faa1a-117">Setting Definition Id</span></span>|
|<span data-ttu-id="faa1a-118">isRequired</span><span class="sxs-lookup"><span data-stu-id="faa1a-118">isRequired</span></span>|<span data-ttu-id="faa1a-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="faa1a-119">Boolean</span></span>|<span data-ttu-id="faa1a-120">Indica se uma política deve especificar essa configuração.</span><span class="sxs-lookup"><span data-stu-id="faa1a-120">Indicates if a policy must specify this setting.</span></span>|

## <a name="relationships"></a><span data-ttu-id="faa1a-121">Relações</span><span class="sxs-lookup"><span data-stu-id="faa1a-121">Relationships</span></span>
<span data-ttu-id="faa1a-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="faa1a-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="faa1a-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="faa1a-123">JSON Representation</span></span>
<span data-ttu-id="faa1a-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="faa1a-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingInstanceTemplate",
  "settingInstanceTemplateId": "String",
  "settingDefinitionId": "String",
  "isRequired": true
}
```




