---
title: tipo de recurso windowsEnrollmentStatusScreenSettings
description: Configuração da tela status do registro
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b47d24b7bec3b20b23077e34b36a9f9e95387789
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43358128"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="0b544-103">tipo de recurso windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="0b544-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

<span data-ttu-id="0b544-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b544-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0b544-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="0b544-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0b544-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="0b544-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0b544-107">Configuração da tela status do registro</span><span class="sxs-lookup"><span data-stu-id="0b544-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="0b544-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="0b544-108">Properties</span></span>
|<span data-ttu-id="0b544-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="0b544-109">Property</span></span>|<span data-ttu-id="0b544-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="0b544-110">Type</span></span>|<span data-ttu-id="0b544-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="0b544-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0b544-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="0b544-112">hideInstallationProgress</span></span>|<span data-ttu-id="0b544-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b544-113">Boolean</span></span>|<span data-ttu-id="0b544-114">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="0b544-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="0b544-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="0b544-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="0b544-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b544-116">Boolean</span></span>|<span data-ttu-id="0b544-117">Permitir ou bloquear o usuário para usar dispositivo antes da conclusão da instalação de perfil e aplicativo</span><span class="sxs-lookup"><span data-stu-id="0b544-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="0b544-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="0b544-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="0b544-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b544-119">Boolean</span></span>|<span data-ttu-id="0b544-120">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="0b544-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="0b544-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="0b544-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="0b544-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b544-122">Boolean</span></span>|<span data-ttu-id="0b544-123">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="0b544-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="0b544-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="0b544-124">customErrorMessage</span></span>|<span data-ttu-id="0b544-125">String</span><span class="sxs-lookup"><span data-stu-id="0b544-125">String</span></span>|<span data-ttu-id="0b544-126">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="0b544-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="0b544-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="0b544-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="0b544-128">Int32</span><span class="sxs-lookup"><span data-stu-id="0b544-128">Int32</span></span>|<span data-ttu-id="0b544-129">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="0b544-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="0b544-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="0b544-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="0b544-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="0b544-131">Boolean</span></span>|<span data-ttu-id="0b544-132">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="0b544-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="0b544-133">Relações</span><span class="sxs-lookup"><span data-stu-id="0b544-133">Relationships</span></span>
<span data-ttu-id="0b544-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="0b544-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="0b544-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="0b544-135">JSON Representation</span></span>
<span data-ttu-id="0b544-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="0b544-136">Here is a JSON representation of the resource.</span></span>
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



