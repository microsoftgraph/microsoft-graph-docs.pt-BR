---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a08a4194fe06cbfe612d1127b28fd34c877da715
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42780868"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="a39cf-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a39cf-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="a39cf-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a39cf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a39cf-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a39cf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a39cf-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="a39cf-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="a39cf-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a39cf-107">Properties</span></span>
|<span data-ttu-id="a39cf-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a39cf-108">Property</span></span>|<span data-ttu-id="a39cf-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="a39cf-109">Type</span></span>|<span data-ttu-id="a39cf-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a39cf-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a39cf-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="a39cf-111">subjectName</span></span>|<span data-ttu-id="a39cf-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a39cf-112">String</span></span>|<span data-ttu-id="a39cf-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a39cf-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="a39cf-114">description</span><span class="sxs-lookup"><span data-stu-id="a39cf-114">description</span></span>|<span data-ttu-id="a39cf-115">String</span><span class="sxs-lookup"><span data-stu-id="a39cf-115">String</span></span>|<span data-ttu-id="a39cf-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a39cf-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="a39cf-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a39cf-117">expirationDateTime</span></span>|<span data-ttu-id="a39cf-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a39cf-118">DateTimeOffset</span></span>|<span data-ttu-id="a39cf-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a39cf-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="a39cf-120">certificado</span><span class="sxs-lookup"><span data-stu-id="a39cf-120">certificate</span></span>|<span data-ttu-id="a39cf-121">Binário</span><span class="sxs-lookup"><span data-stu-id="a39cf-121">Binary</span></span>|<span data-ttu-id="a39cf-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a39cf-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a39cf-123">Relações</span><span class="sxs-lookup"><span data-stu-id="a39cf-123">Relationships</span></span>
<span data-ttu-id="a39cf-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a39cf-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a39cf-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a39cf-125">JSON Representation</span></span>
<span data-ttu-id="a39cf-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a39cf-126">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```



