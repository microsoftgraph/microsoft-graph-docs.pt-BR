---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: f49f5651c6e4f7bea1eb4650e9252c397cc2a930
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42533321"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="ff47c-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="ff47c-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

<span data-ttu-id="ff47c-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff47c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff47c-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ff47c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff47c-106">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="ff47c-106">Windows Information Protection DataRecoveryCertificate</span></span>

## <a name="properties"></a><span data-ttu-id="ff47c-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ff47c-107">Properties</span></span>
|<span data-ttu-id="ff47c-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ff47c-108">Property</span></span>|<span data-ttu-id="ff47c-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ff47c-109">Type</span></span>|<span data-ttu-id="ff47c-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ff47c-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ff47c-111">SubjectName</span><span class="sxs-lookup"><span data-stu-id="ff47c-111">subjectName</span></span>|<span data-ttu-id="ff47c-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ff47c-112">String</span></span>|<span data-ttu-id="ff47c-113">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="ff47c-113">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="ff47c-114">description</span><span class="sxs-lookup"><span data-stu-id="ff47c-114">description</span></span>|<span data-ttu-id="ff47c-115">String</span><span class="sxs-lookup"><span data-stu-id="ff47c-115">String</span></span>|<span data-ttu-id="ff47c-116">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="ff47c-116">Data recovery Certificate description</span></span>|
|<span data-ttu-id="ff47c-117">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ff47c-117">expirationDateTime</span></span>|<span data-ttu-id="ff47c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ff47c-118">DateTimeOffset</span></span>|<span data-ttu-id="ff47c-119">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="ff47c-119">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="ff47c-120">certificado</span><span class="sxs-lookup"><span data-stu-id="ff47c-120">certificate</span></span>|<span data-ttu-id="ff47c-121">Binário</span><span class="sxs-lookup"><span data-stu-id="ff47c-121">Binary</span></span>|<span data-ttu-id="ff47c-122">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="ff47c-122">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="ff47c-123">Relações</span><span class="sxs-lookup"><span data-stu-id="ff47c-123">Relationships</span></span>
<span data-ttu-id="ff47c-124">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ff47c-124">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ff47c-125">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ff47c-125">JSON Representation</span></span>
<span data-ttu-id="ff47c-126">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ff47c-126">Here is a JSON representation of the resource.</span></span>
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




