---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a7253d8e40ef699bc1066c57c4c423c79a069142
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/31/2019
ms.locfileid: "35967893"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="1604a-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="1604a-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="1604a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1604a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1604a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1604a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1604a-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="1604a-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="1604a-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1604a-107">Properties</span></span>
|<span data-ttu-id="1604a-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1604a-108">Property</span></span>|<span data-ttu-id="1604a-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="1604a-109">Type</span></span>|<span data-ttu-id="1604a-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="1604a-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1604a-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="1604a-111">subjectName</span></span>|<span data-ttu-id="1604a-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1604a-112">String</span></span>|<span data-ttu-id="1604a-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1604a-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="1604a-114">descrição</span><span class="sxs-lookup"><span data-stu-id="1604a-114">description</span></span>|<span data-ttu-id="1604a-115">String</span><span class="sxs-lookup"><span data-stu-id="1604a-115">String</span></span>|<span data-ttu-id="1604a-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1604a-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="1604a-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="1604a-117">expirationDateTime</span></span>|<span data-ttu-id="1604a-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1604a-118">DateTimeOffset</span></span>|<span data-ttu-id="1604a-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1604a-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="1604a-120">certificado</span><span class="sxs-lookup"><span data-stu-id="1604a-120">certificate</span></span>|<span data-ttu-id="1604a-121">Binário</span><span class="sxs-lookup"><span data-stu-id="1604a-121">Binary</span></span>|<span data-ttu-id="1604a-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="1604a-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="1604a-123">Relações</span><span class="sxs-lookup"><span data-stu-id="1604a-123">Relationships</span></span>
<span data-ttu-id="1604a-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1604a-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="1604a-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1604a-125">JSON Representation</span></span>
<span data-ttu-id="1604a-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1604a-126">Here is a JSON representation of the resource.</span></span>
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





