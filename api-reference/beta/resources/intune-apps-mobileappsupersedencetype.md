---
title: tipo de enumeração mobileAppSupersedenceType
description: Indica o tipo de substituição associado a uma relação entre dois aplicativos móveis.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: enumPageType
ms.openlocfilehash: f475d32aa8ef4427eada5a049e54c8f3a73e3018
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217071"
---
# <a name="mobileappsupersedencetype-enum-type"></a><span data-ttu-id="412c8-103">tipo de enumeração mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="412c8-103">mobileAppSupersedenceType enum type</span></span>

<span data-ttu-id="412c8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="412c8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="412c8-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="412c8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="412c8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="412c8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="412c8-107">Indica o tipo de substituição associado a uma relação entre dois aplicativos móveis.</span><span class="sxs-lookup"><span data-stu-id="412c8-107">Indicates the supersedence type associated with a relationship between two mobile apps.</span></span>

## <a name="members"></a><span data-ttu-id="412c8-108">Membros</span><span class="sxs-lookup"><span data-stu-id="412c8-108">Members</span></span>
|<span data-ttu-id="412c8-109">Membro</span><span class="sxs-lookup"><span data-stu-id="412c8-109">Member</span></span>|<span data-ttu-id="412c8-110">Valor</span><span class="sxs-lookup"><span data-stu-id="412c8-110">Value</span></span>|<span data-ttu-id="412c8-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="412c8-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="412c8-112">cumulativo</span><span class="sxs-lookup"><span data-stu-id="412c8-112">update</span></span>|<span data-ttu-id="412c8-113">,0</span><span class="sxs-lookup"><span data-stu-id="412c8-113">0</span></span>|<span data-ttu-id="412c8-114">Indica que o aplicativo filho deve ser atualizado pela lógica interna do aplicativo pai.</span><span class="sxs-lookup"><span data-stu-id="412c8-114">Indicates that the child app should be updated by the internal logic of the parent app.</span></span>|
|<span data-ttu-id="412c8-115">replace</span><span class="sxs-lookup"><span data-stu-id="412c8-115">replace</span></span>|<span data-ttu-id="412c8-116">1</span><span class="sxs-lookup"><span data-stu-id="412c8-116">1</span></span>|<span data-ttu-id="412c8-117">Indica que o aplicativo filho deve ser desinstalado antes da instalação do aplicativo pai.</span><span class="sxs-lookup"><span data-stu-id="412c8-117">Indicates that the child app should be uninstalled before installing the parent app.</span></span>|




