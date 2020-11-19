---
title: tipo de recurso windows10XCustomSubjectAlternativeName
description: Tipo de perfil básico para certificados de autenticação (SCEP ou PFX de criação)
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 725d2cc13db1cb28b9286479f201b9bb38f6eefa
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301377"
---
# <a name="windows10xcustomsubjectalternativename-resource-type"></a><span data-ttu-id="34bd7-103">tipo de recurso windows10XCustomSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="34bd7-103">windows10XCustomSubjectAlternativeName resource type</span></span>

<span data-ttu-id="34bd7-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="34bd7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="34bd7-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="34bd7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="34bd7-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="34bd7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="34bd7-107">Tipo de perfil básico para certificados de autenticação (SCEP ou PFX de criação)</span><span class="sxs-lookup"><span data-stu-id="34bd7-107">Base Profile Type for Authentication Certificates (SCEP or PFX Create)</span></span>

## <a name="properties"></a><span data-ttu-id="34bd7-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34bd7-108">Properties</span></span>
|<span data-ttu-id="34bd7-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34bd7-109">Property</span></span>|<span data-ttu-id="34bd7-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="34bd7-110">Type</span></span>|<span data-ttu-id="34bd7-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="34bd7-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="34bd7-112">sanType</span><span class="sxs-lookup"><span data-stu-id="34bd7-112">sanType</span></span>|[<span data-ttu-id="34bd7-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="34bd7-113">subjectAlternativeNameType</span></span>](../resources/intune-shared-subjectalternativenametype.md)|<span data-ttu-id="34bd7-114">Tipo de SAN personalizado.</span><span class="sxs-lookup"><span data-stu-id="34bd7-114">Custom SAN Type.</span></span> <span data-ttu-id="34bd7-115">Os possíveis valores são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span><span class="sxs-lookup"><span data-stu-id="34bd7-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`, `universalResourceIdentifier`.</span></span>|
|<span data-ttu-id="34bd7-116">nome</span><span class="sxs-lookup"><span data-stu-id="34bd7-116">name</span></span>|<span data-ttu-id="34bd7-117">String</span><span class="sxs-lookup"><span data-stu-id="34bd7-117">String</span></span>|<span data-ttu-id="34bd7-118">Nome da SAN personalizada</span><span class="sxs-lookup"><span data-stu-id="34bd7-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="34bd7-119">Relações</span><span class="sxs-lookup"><span data-stu-id="34bd7-119">Relationships</span></span>
<span data-ttu-id="34bd7-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34bd7-120">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="34bd7-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34bd7-121">JSON Representation</span></span>
<span data-ttu-id="34bd7-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34bd7-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10XCustomSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10XCustomSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```




