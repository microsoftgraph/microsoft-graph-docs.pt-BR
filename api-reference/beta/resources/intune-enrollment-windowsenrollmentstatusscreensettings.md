---
title: tipo de recurso de windowsEnrollmentStatusScreenSettings
description: Configuração de tela do status de inscrição
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e5ffb2827988b80b4d6563d8a92c9ccea7ac9828
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29399931"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="65c64-103">tipo de recurso de windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="65c64-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="65c64-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="65c64-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="65c64-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="65c64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="65c64-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="65c64-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65c64-107">Configuração de tela do status de inscrição</span><span class="sxs-lookup"><span data-stu-id="65c64-107">Enrollment status screen setting</span></span>

## <a name="properties"></a><span data-ttu-id="65c64-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="65c64-108">Properties</span></span>
|<span data-ttu-id="65c64-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="65c64-109">Property</span></span>|<span data-ttu-id="65c64-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="65c64-110">Type</span></span>|<span data-ttu-id="65c64-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="65c64-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c64-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="65c64-112">hideInstallationProgress</span></span>|<span data-ttu-id="65c64-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c64-113">Boolean</span></span>|<span data-ttu-id="65c64-114">Mostrar ou ocultar o progresso da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="65c64-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="65c64-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="65c64-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="65c64-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c64-116">Boolean</span></span>|<span data-ttu-id="65c64-117">Permitir ou bloquear um usuário utilize um dispositivo antes da instalação de perfil e o aplicativo completo</span><span class="sxs-lookup"><span data-stu-id="65c64-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="65c64-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="65c64-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="65c64-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c64-119">Boolean</span></span>|<span data-ttu-id="65c64-120">Permitir que o usuário repetir a instalação em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="65c64-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="65c64-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="65c64-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="65c64-122">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c64-122">Boolean</span></span>|<span data-ttu-id="65c64-123">Permitir ou bloquear o conjunto de log em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="65c64-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="65c64-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="65c64-124">customErrorMessage</span></span>|<span data-ttu-id="65c64-125">String</span><span class="sxs-lookup"><span data-stu-id="65c64-125">String</span></span>|<span data-ttu-id="65c64-126">Definir a mensagem de erro personalizada para mostrar após a falha de instalação</span><span class="sxs-lookup"><span data-stu-id="65c64-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="65c64-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="65c64-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="65c64-128">Int32</span><span class="sxs-lookup"><span data-stu-id="65c64-128">Int32</span></span>|<span data-ttu-id="65c64-129">Definir tempo limite de progresso de instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="65c64-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="65c64-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="65c64-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="65c64-131">Boolean</span><span class="sxs-lookup"><span data-stu-id="65c64-131">Boolean</span></span>|<span data-ttu-id="65c64-132">Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="65c64-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="65c64-133">Relações</span><span class="sxs-lookup"><span data-stu-id="65c64-133">Relationships</span></span>
<span data-ttu-id="65c64-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="65c64-134">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="65c64-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="65c64-135">JSON Representation</span></span>
<span data-ttu-id="65c64-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="65c64-136">Here is a JSON representation of the resource.</span></span>
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




