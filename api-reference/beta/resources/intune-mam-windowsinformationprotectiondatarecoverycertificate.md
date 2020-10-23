---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a4ad031e97d6511280517ef1e9c3b30141c7125c
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/22/2020
ms.locfileid: "48727180"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="2b0de-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2b0de-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="2b0de-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2b0de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2b0de-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2b0de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2b0de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2b0de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2b0de-107">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="2b0de-107">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="2b0de-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b0de-108">Properties</span></span>
|<span data-ttu-id="2b0de-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b0de-109">Property</span></span>|<span data-ttu-id="2b0de-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b0de-110">Type</span></span>|<span data-ttu-id="2b0de-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b0de-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b0de-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="2b0de-112">subjectName</span></span>|<span data-ttu-id="2b0de-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b0de-113">String</span></span>|<span data-ttu-id="2b0de-114">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b0de-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="2b0de-115">description</span><span class="sxs-lookup"><span data-stu-id="2b0de-115">description</span></span>|<span data-ttu-id="2b0de-116">String</span><span class="sxs-lookup"><span data-stu-id="2b0de-116">String</span></span>|<span data-ttu-id="2b0de-117">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b0de-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="2b0de-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2b0de-118">expirationDateTime</span></span>|<span data-ttu-id="2b0de-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b0de-119">DateTimeOffset</span></span>|<span data-ttu-id="2b0de-120">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b0de-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="2b0de-121">certificado</span><span class="sxs-lookup"><span data-stu-id="2b0de-121">certificate</span></span>|<span data-ttu-id="2b0de-122">Binário</span><span class="sxs-lookup"><span data-stu-id="2b0de-122">Binary</span></span>|<span data-ttu-id="2b0de-123">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b0de-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b0de-124">Relações</span><span class="sxs-lookup"><span data-stu-id="2b0de-124">Relationships</span></span>
<span data-ttu-id="2b0de-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b0de-125">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b0de-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b0de-126">JSON Representation</span></span>
<span data-ttu-id="2b0de-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b0de-127">Here is a JSON representation of the resource.</span></span>
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





