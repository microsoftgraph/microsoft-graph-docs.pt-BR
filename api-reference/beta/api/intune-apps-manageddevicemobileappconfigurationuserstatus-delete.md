---
title: Excluir managedDeviceMobileAppConfigurationUserStatus
description: Exclui managedDeviceMobileAppConfigurationUserStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 52a6b6025ebe6ba56895850674a0a11cafec488e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397880"
---
# <a name="delete-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="ba351-103">Excluir managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="ba351-103">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>

> <span data-ttu-id="ba351-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="ba351-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ba351-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ba351-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ba351-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="ba351-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba351-107">Exclui [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="ba351-107">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba351-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ba351-108">Prerequisites</span></span>
<span data-ttu-id="ba351-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="ba351-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ba351-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ba351-111">Permission type</span></span>|<span data-ttu-id="ba351-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ba351-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba351-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ba351-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ba351-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ba351-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ba351-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ba351-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba351-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba351-116">Not supported.</span></span>|
|<span data-ttu-id="ba351-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ba351-117">Application</span></span>|<span data-ttu-id="ba351-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ba351-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba351-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ba351-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ba351-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ba351-120">Request headers</span></span>
|<span data-ttu-id="ba351-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ba351-121">Header</span></span>|<span data-ttu-id="ba351-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ba351-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba351-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ba351-123">Authorization</span></span>|<span data-ttu-id="ba351-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ba351-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba351-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ba351-125">Accept</span></span>|<span data-ttu-id="ba351-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ba351-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba351-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ba351-127">Request body</span></span>
<span data-ttu-id="ba351-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="ba351-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba351-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba351-129">Response</span></span>
<span data-ttu-id="ba351-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="ba351-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ba351-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ba351-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba351-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ba351-132">Request</span></span>
<span data-ttu-id="ba351-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ba351-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="ba351-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="ba351-134">Response</span></span>
<span data-ttu-id="ba351-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ba351-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




