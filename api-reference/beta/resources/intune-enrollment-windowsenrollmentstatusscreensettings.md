---
title: tipo de recurso windowsEnrollmentStatusScreenSettings
description: Configuração da tela status do registro
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3758dd850a5c98ea2c0ddad4d261fc9a7388ac3c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42528225"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="d8934-103">tipo de recurso windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="d8934-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

<span data-ttu-id="d8934-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="d8934-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8934-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d8934-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8934-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d8934-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8934-107">Configuração da tela status do registro</span><span class="sxs-lookup"><span data-stu-id="d8934-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="d8934-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d8934-108">Properties</span></span>
|<span data-ttu-id="d8934-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d8934-109">Property</span></span>|<span data-ttu-id="d8934-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="d8934-110">Type</span></span>|<span data-ttu-id="d8934-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="d8934-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8934-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="d8934-112">hideInstallationProgress</span></span>|<span data-ttu-id="d8934-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8934-113">Boolean</span></span>|<span data-ttu-id="d8934-114">Mostrar ou ocultar o andamento da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="d8934-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="d8934-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="d8934-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="d8934-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8934-116">Boolean</span></span>|<span data-ttu-id="d8934-117">Permitir ou bloquear o usuário para usar dispositivo antes da conclusão da instalação de perfil e aplicativo</span><span class="sxs-lookup"><span data-stu-id="d8934-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="d8934-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="d8934-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="d8934-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8934-119">Boolean</span></span>|<span data-ttu-id="d8934-120">Permitir que o usuário repita a configuração após a instalação falhar</span><span class="sxs-lookup"><span data-stu-id="d8934-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="d8934-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d8934-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="d8934-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8934-122">Boolean</span></span>|<span data-ttu-id="d8934-123">Permitir ou bloquear coleta de log na falha de instalação</span><span class="sxs-lookup"><span data-stu-id="d8934-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="d8934-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="d8934-124">customErrorMessage</span></span>|<span data-ttu-id="d8934-125">String</span><span class="sxs-lookup"><span data-stu-id="d8934-125">String</span></span>|<span data-ttu-id="d8934-126">Definir uma mensagem de erro personalizada para mostrar após falha da instalação</span><span class="sxs-lookup"><span data-stu-id="d8934-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="d8934-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="d8934-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="d8934-128">Int32</span><span class="sxs-lookup"><span data-stu-id="d8934-128">Int32</span></span>|<span data-ttu-id="d8934-129">Definir o tempo limite de progresso da instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="d8934-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="d8934-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="d8934-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="d8934-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="d8934-131">Boolean</span></span>|<span data-ttu-id="d8934-132">Permitir que o usuário continue usando o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="d8934-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="d8934-133">Relações</span><span class="sxs-lookup"><span data-stu-id="d8934-133">Relationships</span></span>
<span data-ttu-id="d8934-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d8934-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d8934-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d8934-135">JSON Representation</span></span>
<span data-ttu-id="d8934-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d8934-136">Here is a JSON representation of the resource.</span></span>
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



