---
title: Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference
description: Definindo informações de referência do modelo de valor
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: fa4ecc07044d90bfc869467de8e8249f7581e228
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/26/2021
ms.locfileid: "52666769"
---
# <a name="devicemanagementconfigurationsettingvaluetemplatereference-resource-type"></a><span data-ttu-id="07755-103">Tipo de recurso deviceManagementConfigurationSettingValueTemplateReference</span><span class="sxs-lookup"><span data-stu-id="07755-103">deviceManagementConfigurationSettingValueTemplateReference resource type</span></span>

<span data-ttu-id="07755-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07755-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07755-105">**Importante:** As APIs Graph Microsoft na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="07755-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="07755-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="07755-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07755-107">Definindo informações de referência do modelo de valor</span><span class="sxs-lookup"><span data-stu-id="07755-107">Setting value template reference information</span></span>

## <a name="properties"></a><span data-ttu-id="07755-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="07755-108">Properties</span></span>
|<span data-ttu-id="07755-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="07755-109">Property</span></span>|<span data-ttu-id="07755-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="07755-110">Type</span></span>|<span data-ttu-id="07755-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="07755-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07755-112">settingValueTemplateId</span><span class="sxs-lookup"><span data-stu-id="07755-112">settingValueTemplateId</span></span>|<span data-ttu-id="07755-113">String</span><span class="sxs-lookup"><span data-stu-id="07755-113">String</span></span>|<span data-ttu-id="07755-114">Definindo a id do modelo de valor</span><span class="sxs-lookup"><span data-stu-id="07755-114">Setting value template id</span></span>|
|<span data-ttu-id="07755-115">useTemplateDefault</span><span class="sxs-lookup"><span data-stu-id="07755-115">useTemplateDefault</span></span>|<span data-ttu-id="07755-116">Booleano</span><span class="sxs-lookup"><span data-stu-id="07755-116">Boolean</span></span>|<span data-ttu-id="07755-117">Indica se o valor de configuração da política deve ser atualizado para corresponder ao valor padrão da configuração do modelo</span><span class="sxs-lookup"><span data-stu-id="07755-117">Indicates whether to update policy setting value to match template setting default value</span></span>|

## <a name="relationships"></a><span data-ttu-id="07755-118">Relações</span><span class="sxs-lookup"><span data-stu-id="07755-118">Relationships</span></span>
<span data-ttu-id="07755-119">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="07755-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="07755-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="07755-120">JSON Representation</span></span>
<span data-ttu-id="07755-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="07755-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementConfigurationSettingValueTemplateReference",
  "settingValueTemplateId": "String",
  "useTemplateDefault": true
}
```




