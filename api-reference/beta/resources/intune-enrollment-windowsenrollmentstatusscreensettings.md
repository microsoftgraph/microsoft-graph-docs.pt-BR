---
title: tipo de recurso windowsEnrollmentStatusScreenSettings
description: Configuração da tela status do registro
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d22f7497fb79921bbbf34c6f3334ccc2ae4d7d53
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/14/2019
ms.locfileid: "34994899"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="c096d-103">tipo de recurso windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="c096d-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="c096d-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="c096d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c096d-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="c096d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c096d-106">Configuração da tela status do registro</span><span class="sxs-lookup"><span data-stu-id="c096d-106">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="c096d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c096d-107">Properties</span></span>
|<span data-ttu-id="c096d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c096d-108">Property</span></span>|<span data-ttu-id="c096d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="c096d-109">Type</span></span>|<span data-ttu-id="c096d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="c096d-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c096d-111">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="c096d-111">hideInstallationProgress</span></span>|<span data-ttu-id="c096d-112">Booliano</span><span class="sxs-lookup"><span data-stu-id="c096d-112">Boolean</span></span>|<span data-ttu-id="c096d-113">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="c096d-113">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="c096d-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="c096d-114">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="c096d-115">Booliano</span><span class="sxs-lookup"><span data-stu-id="c096d-115">Boolean</span></span>|<span data-ttu-id="c096d-116">Permitir ou bloquear o usuário para usar dispositivo antes da conclusão da instalação de perfil e aplicativo</span><span class="sxs-lookup"><span data-stu-id="c096d-116">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="c096d-117">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="c096d-117">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="c096d-118">Booliano</span><span class="sxs-lookup"><span data-stu-id="c096d-118">Boolean</span></span>|<span data-ttu-id="c096d-119">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="c096d-119">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="c096d-120">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="c096d-120">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="c096d-121">Booliano</span><span class="sxs-lookup"><span data-stu-id="c096d-121">Boolean</span></span>|<span data-ttu-id="c096d-122">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="c096d-122">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="c096d-123">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="c096d-123">customErrorMessage</span></span>|<span data-ttu-id="c096d-124">String</span><span class="sxs-lookup"><span data-stu-id="c096d-124">String</span></span>|<span data-ttu-id="c096d-125">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="c096d-125">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="c096d-126">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="c096d-126">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="c096d-127">Int32</span><span class="sxs-lookup"><span data-stu-id="c096d-127">Int32</span></span>|<span data-ttu-id="c096d-128">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="c096d-128">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="c096d-129">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="c096d-129">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="c096d-130">Booliano</span><span class="sxs-lookup"><span data-stu-id="c096d-130">Boolean</span></span>|<span data-ttu-id="c096d-131">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="c096d-131">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="c096d-132">Relações</span><span class="sxs-lookup"><span data-stu-id="c096d-132">Relationships</span></span>
<span data-ttu-id="c096d-133">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c096d-133">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="c096d-134">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c096d-134">JSON Representation</span></span>
<span data-ttu-id="c096d-135">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c096d-135">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsEnrollmentStatusScreenSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsEnrollmentStatusScreenSettings",
  "hideInstallationProgress": true,
  "allowDeviceUseBeforeProfileAndAppInstallComplete": true,
  "blockDeviceSetupRetryByUser": true,
  "allowLogCollectionOnInstallFailure": true,
  "customErrorMessage": "String",
  "installProgressTimeoutInMinutes": 1024,
  "allowDeviceUseOnInstallFailure": true
}
```





