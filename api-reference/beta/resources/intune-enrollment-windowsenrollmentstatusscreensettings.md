---
title: tipo de recurso de windowsEnrollmentStatusScreenSettings
description: Configuração de tela do status de inscrição
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 7263fdd8ab3d9a39d5081322c62cfcf76a4c7aa0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877445"
---
# <a name="windowsenrollmentstatusscreensettings-resource-type"></a><span data-ttu-id="8f6dc-103">tipo de recurso de windowsEnrollmentStatusScreenSettings</span><span class="sxs-lookup"><span data-stu-id="8f6dc-103">windowsEnrollmentStatusScreenSettings resource type</span></span>

> <span data-ttu-id="8f6dc-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f6dc-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8f6dc-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f6dc-107">Configuração de tela do status de inscrição</span><span class="sxs-lookup"><span data-stu-id="8f6dc-107">Enrollment status screen setting</span></span>
## <a name="properties"></a><span data-ttu-id="8f6dc-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f6dc-108">Properties</span></span>
|<span data-ttu-id="8f6dc-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f6dc-109">Property</span></span>|<span data-ttu-id="8f6dc-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f6dc-110">Type</span></span>|<span data-ttu-id="8f6dc-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f6dc-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8f6dc-112">hideInstallationProgress</span><span class="sxs-lookup"><span data-stu-id="8f6dc-112">hideInstallationProgress</span></span>|<span data-ttu-id="8f6dc-113">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f6dc-113">Boolean</span></span>|<span data-ttu-id="8f6dc-114">Mostrar ou ocultar o progresso da instalação para o usuário</span><span class="sxs-lookup"><span data-stu-id="8f6dc-114">Show or hide installation progress to user</span></span>|
|<span data-ttu-id="8f6dc-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span><span class="sxs-lookup"><span data-stu-id="8f6dc-115">allowDeviceUseBeforeProfileAndAppInstallComplete</span></span>|<span data-ttu-id="8f6dc-116">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f6dc-116">Boolean</span></span>|<span data-ttu-id="8f6dc-117">Permitir ou bloquear um usuário utilize um dispositivo antes da instalação de perfil e o aplicativo completo</span><span class="sxs-lookup"><span data-stu-id="8f6dc-117">Allow or block user to use device before profile and app installation complete</span></span>|
|<span data-ttu-id="8f6dc-118">blockDeviceSetupRetryByUser</span><span class="sxs-lookup"><span data-stu-id="8f6dc-118">blockDeviceSetupRetryByUser</span></span>|<span data-ttu-id="8f6dc-119">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f6dc-119">Boolean</span></span>|<span data-ttu-id="8f6dc-120">Permitir que o usuário repetir a instalação em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-120">Allow the user to retry the setup on installation failure</span></span>|
|<span data-ttu-id="8f6dc-121">allowLogCollectionOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="8f6dc-121">allowLogCollectionOnInstallFailure</span></span>|<span data-ttu-id="8f6dc-122">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f6dc-122">Boolean</span></span>|<span data-ttu-id="8f6dc-123">Permitir ou bloquear o conjunto de log em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-123">Allow or block log collection on installation failure</span></span>|
|<span data-ttu-id="8f6dc-124">customErrorMessage</span><span class="sxs-lookup"><span data-stu-id="8f6dc-124">customErrorMessage</span></span>|<span data-ttu-id="8f6dc-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f6dc-125">String</span></span>|<span data-ttu-id="8f6dc-126">Definir a mensagem de erro personalizada para mostrar após a falha de instalação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-126">Set custom error message to show upon installation failure</span></span>|
|<span data-ttu-id="8f6dc-127">installProgressTimeoutInMinutes</span><span class="sxs-lookup"><span data-stu-id="8f6dc-127">installProgressTimeoutInMinutes</span></span>|<span data-ttu-id="8f6dc-128">Int32</span><span class="sxs-lookup"><span data-stu-id="8f6dc-128">Int32</span></span>|<span data-ttu-id="8f6dc-129">Definir tempo limite de progresso de instalação em minutos</span><span class="sxs-lookup"><span data-stu-id="8f6dc-129">Set installation progress timeout in minutes</span></span>|
|<span data-ttu-id="8f6dc-130">allowDeviceUseOnInstallFailure</span><span class="sxs-lookup"><span data-stu-id="8f6dc-130">allowDeviceUseOnInstallFailure</span></span>|<span data-ttu-id="8f6dc-131">Booliano</span><span class="sxs-lookup"><span data-stu-id="8f6dc-131">Boolean</span></span>|<span data-ttu-id="8f6dc-132">Permitir que o usuário continue a usar o dispositivo em caso de falha de instalação</span><span class="sxs-lookup"><span data-stu-id="8f6dc-132">Allow the user to continue using the device on installation failure</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f6dc-133">Relações</span><span class="sxs-lookup"><span data-stu-id="8f6dc-133">Relationships</span></span>
<span data-ttu-id="8f6dc-134">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f6dc-134">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8f6dc-135">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f6dc-135">JSON Representation</span></span>
<span data-ttu-id="8f6dc-136">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f6dc-136">Here is a JSON representation of the resource.</span></span>
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





