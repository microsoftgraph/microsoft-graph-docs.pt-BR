---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 555cac098d2796f612054f11e2c5ade525ad6199
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "36037727"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="c3127-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="c3127-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="c3127-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c3127-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3127-105">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="c3127-105">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="c3127-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c3127-106">Properties</span></span>
|<span data-ttu-id="c3127-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c3127-107">Property</span></span>|<span data-ttu-id="c3127-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="c3127-108">Type</span></span>|<span data-ttu-id="c3127-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="c3127-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3127-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="c3127-110">subjectName</span></span>|<span data-ttu-id="c3127-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c3127-111">String</span></span>|<span data-ttu-id="c3127-112">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="c3127-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="c3127-113">descrição</span><span class="sxs-lookup"><span data-stu-id="c3127-113">description</span></span>|<span data-ttu-id="c3127-114">String</span><span class="sxs-lookup"><span data-stu-id="c3127-114">String</span></span>|<span data-ttu-id="c3127-115">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="c3127-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="c3127-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="c3127-116">expirationDateTime</span></span>|<span data-ttu-id="c3127-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c3127-117">DateTimeOffset</span></span>|<span data-ttu-id="c3127-118">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="c3127-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="c3127-119">certificado</span><span class="sxs-lookup"><span data-stu-id="c3127-119">certificate</span></span>|<span data-ttu-id="c3127-120">Binário</span><span class="sxs-lookup"><span data-stu-id="c3127-120">Binary</span></span>|<span data-ttu-id="c3127-121">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="c3127-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="c3127-122">Relações</span><span class="sxs-lookup"><span data-stu-id="c3127-122">Relationships</span></span>
<span data-ttu-id="c3127-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c3127-123">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3127-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c3127-124">JSON Representation</span></span>
<span data-ttu-id="c3127-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c3127-125">Here is a JSON representation of the resource.</span></span>
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



