---
title: tipo de recurso de customSubjectAlternativeName
description: Definição de nome alternativo da entidade personalizada
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: b3f081b37b79be45d6705d24be58ea7295b58b68
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415667"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="3fec5-103">tipo de recurso de customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="3fec5-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="3fec5-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="3fec5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="3fec5-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="3fec5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3fec5-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="3fec5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3fec5-107">Definição de nome alternativo da entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="3fec5-107">Custom Subject Alternative Name definition</span></span>

## <a name="properties"></a><span data-ttu-id="3fec5-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="3fec5-108">Properties</span></span>
|<span data-ttu-id="3fec5-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3fec5-109">Property</span></span>|<span data-ttu-id="3fec5-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="3fec5-110">Type</span></span>|<span data-ttu-id="3fec5-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="3fec5-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3fec5-112">sanType</span><span class="sxs-lookup"><span data-stu-id="3fec5-112">sanType</span></span>|[<span data-ttu-id="3fec5-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="3fec5-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="3fec5-114">Tipo de SAN personalizado.</span><span class="sxs-lookup"><span data-stu-id="3fec5-114">Custom SAN Type.</span></span> <span data-ttu-id="3fec5-115">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="3fec5-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="3fec5-116">name</span><span class="sxs-lookup"><span data-stu-id="3fec5-116">name</span></span>|<span data-ttu-id="3fec5-117">String</span><span class="sxs-lookup"><span data-stu-id="3fec5-117">String</span></span>|<span data-ttu-id="3fec5-118">Nome de SAN personalizado</span><span class="sxs-lookup"><span data-stu-id="3fec5-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="3fec5-119">Relações</span><span class="sxs-lookup"><span data-stu-id="3fec5-119">Relationships</span></span>
<span data-ttu-id="3fec5-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="3fec5-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3fec5-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="3fec5-121">JSON Representation</span></span>
<span data-ttu-id="3fec5-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="3fec5-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




