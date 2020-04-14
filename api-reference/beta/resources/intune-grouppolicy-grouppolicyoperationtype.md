---
title: tipo de enumeração groupPolicyOperationType
description: Tipo de operação de política de grupo.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: enumPageType
ms.openlocfilehash: a14505e31f9e36a41237a578158d8ddcdbef909b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43446931"
---
# <a name="grouppolicyoperationtype-enum-type"></a><span data-ttu-id="82c7b-103">tipo de enumeração groupPolicyOperationType</span><span class="sxs-lookup"><span data-stu-id="82c7b-103">groupPolicyOperationType enum type</span></span>

<span data-ttu-id="82c7b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="82c7b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="82c7b-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="82c7b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="82c7b-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="82c7b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82c7b-107">Tipo de operação de política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82c7b-107">Type of Group Policy operation.</span></span>

## <a name="members"></a><span data-ttu-id="82c7b-108">Membros</span><span class="sxs-lookup"><span data-stu-id="82c7b-108">Members</span></span>
|<span data-ttu-id="82c7b-109">Membro</span><span class="sxs-lookup"><span data-stu-id="82c7b-109">Member</span></span>|<span data-ttu-id="82c7b-110">Valor</span><span class="sxs-lookup"><span data-stu-id="82c7b-110">Value</span></span>|<span data-ttu-id="82c7b-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="82c7b-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82c7b-112">nenhuma</span><span class="sxs-lookup"><span data-stu-id="82c7b-112">none</span></span>|<span data-ttu-id="82c7b-113">,0</span><span class="sxs-lookup"><span data-stu-id="82c7b-113">0</span></span>|<span data-ttu-id="82c7b-114">Tipo de operação inválido da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82c7b-114">Group Policy invalid operation type.</span></span>|
|<span data-ttu-id="82c7b-115">carregar</span><span class="sxs-lookup"><span data-stu-id="82c7b-115">upload</span></span>|<span data-ttu-id="82c7b-116">1</span><span class="sxs-lookup"><span data-stu-id="82c7b-116">1</span></span>|<span data-ttu-id="82c7b-117">Tipo de operação de upload da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82c7b-117">Group Policy upload operation type.</span></span>|
|<span data-ttu-id="82c7b-118">uploadNewVersion</span><span class="sxs-lookup"><span data-stu-id="82c7b-118">uploadNewVersion</span></span>|<span data-ttu-id="82c7b-119">duas</span><span class="sxs-lookup"><span data-stu-id="82c7b-119">2</span></span>|<span data-ttu-id="82c7b-120">Tipo de operação do carregamento da nova versão da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82c7b-120">Group Policy upload new version operation type.</span></span>|
|<span data-ttu-id="82c7b-121">addLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="82c7b-121">addLanguageFiles</span></span>|<span data-ttu-id="82c7b-122">3D</span><span class="sxs-lookup"><span data-stu-id="82c7b-122">3</span></span>|<span data-ttu-id="82c7b-123">Tipo de operação de arquivo de adição de arquivos ADML (novo idioma) da política de grupo.</span><span class="sxs-lookup"><span data-stu-id="82c7b-123">Group Policy add new language(ADML) files operation type.</span></span>|
|<span data-ttu-id="82c7b-124">removeLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="82c7b-124">removeLanguageFiles</span></span>|<span data-ttu-id="82c7b-125">4 </span><span class="sxs-lookup"><span data-stu-id="82c7b-125">4</span></span>|<span data-ttu-id="82c7b-126">Tipo de operação de arquivos ADML (linguagem de remoção de política de grupo).</span><span class="sxs-lookup"><span data-stu-id="82c7b-126">Group Policy remove language(ADML) files operation type.</span></span>|
|<span data-ttu-id="82c7b-127">updateLanguageFiles</span><span class="sxs-lookup"><span data-stu-id="82c7b-127">updateLanguageFiles</span></span>|<span data-ttu-id="82c7b-128">5 </span><span class="sxs-lookup"><span data-stu-id="82c7b-128">5</span></span>|<span data-ttu-id="82c7b-129">Tipo de operação de arquivos ADML (idioma de atualização de política de grupo).</span><span class="sxs-lookup"><span data-stu-id="82c7b-129">Group Policy update language(ADML) files operation type.</span></span>|
|<span data-ttu-id="82c7b-130">remover</span><span class="sxs-lookup"><span data-stu-id="82c7b-130">remove</span></span>|<span data-ttu-id="82c7b-131">6 </span><span class="sxs-lookup"><span data-stu-id="82c7b-131">6</span></span>|<span data-ttu-id="82c7b-132">Política de grupo remover o tipo de operação de arquivo carregado.</span><span class="sxs-lookup"><span data-stu-id="82c7b-132">Group Policy remove uploaded file operation type.</span></span>|



