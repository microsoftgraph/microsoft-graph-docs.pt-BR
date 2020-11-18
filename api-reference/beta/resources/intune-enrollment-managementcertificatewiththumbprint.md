---
title: tipo de recurso managementCertificateWithThumbprint
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: b849da155f0431ba5fd505e04fac23e077753159
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49197874"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="6a3cd-103">tipo de recurso managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="6a3cd-103">managementCertificateWithThumbprint resource type</span></span>

<span data-ttu-id="6a3cd-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a3cd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a3cd-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6a3cd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a3cd-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6a3cd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a3cd-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="6a3cd-107">Not yet documented</span></span>

## <a name="properties"></a><span data-ttu-id="6a3cd-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6a3cd-108">Properties</span></span>
|<span data-ttu-id="6a3cd-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6a3cd-109">Property</span></span>|<span data-ttu-id="6a3cd-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="6a3cd-110">Type</span></span>|<span data-ttu-id="6a3cd-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="6a3cd-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a3cd-112">identificação</span><span class="sxs-lookup"><span data-stu-id="6a3cd-112">thumbprint</span></span>|<span data-ttu-id="6a3cd-113">String</span><span class="sxs-lookup"><span data-stu-id="6a3cd-113">String</span></span>|<span data-ttu-id="6a3cd-114">A impressão digital do certificado de gerenciamento</span><span class="sxs-lookup"><span data-stu-id="6a3cd-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="6a3cd-115">certificado</span><span class="sxs-lookup"><span data-stu-id="6a3cd-115">certificate</span></span>|<span data-ttu-id="6a3cd-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6a3cd-116">String</span></span>|<span data-ttu-id="6a3cd-117">O certificado de gerenciamento codificado base 64</span><span class="sxs-lookup"><span data-stu-id="6a3cd-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="6a3cd-118">Relações</span><span class="sxs-lookup"><span data-stu-id="6a3cd-118">Relationships</span></span>
<span data-ttu-id="6a3cd-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6a3cd-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a3cd-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6a3cd-120">JSON Representation</span></span>
<span data-ttu-id="6a3cd-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6a3cd-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```




