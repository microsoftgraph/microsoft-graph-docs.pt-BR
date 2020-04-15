---
title: Excluir managedDeviceMobileAppConfigurationUserStatus
description: Exclui managedDeviceMobileAppConfigurationUserStatus.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4e7f9db459118866b85efd4331339c10bab99c31
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43471656"
---
# <a name="delete-manageddevicemobileappconfigurationuserstatus"></a><span data-ttu-id="cc795-103">Excluir managedDeviceMobileAppConfigurationUserStatus</span><span class="sxs-lookup"><span data-stu-id="cc795-103">Delete managedDeviceMobileAppConfigurationUserStatus</span></span>

<span data-ttu-id="cc795-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc795-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="cc795-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="cc795-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cc795-106">Exclui [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span><span class="sxs-lookup"><span data-stu-id="cc795-106">Deletes a [managedDeviceMobileAppConfigurationUserStatus](../resources/intune-apps-manageddevicemobileappconfigurationuserstatus.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cc795-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="cc795-107">Prerequisites</span></span>
<span data-ttu-id="cc795-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="cc795-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc795-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="cc795-110">Permission type</span></span>|<span data-ttu-id="cc795-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="cc795-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cc795-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="cc795-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cc795-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cc795-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cc795-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="cc795-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cc795-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc795-115">Not supported.</span></span>|
|<span data-ttu-id="cc795-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="cc795-116">Application</span></span>|<span data-ttu-id="cc795-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="cc795-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cc795-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="cc795-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="cc795-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="cc795-119">Request headers</span></span>
|<span data-ttu-id="cc795-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="cc795-120">Header</span></span>|<span data-ttu-id="cc795-121">Valor</span><span class="sxs-lookup"><span data-stu-id="cc795-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cc795-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="cc795-122">Authorization</span></span>|<span data-ttu-id="cc795-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="cc795-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cc795-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="cc795-124">Accept</span></span>|<span data-ttu-id="cc795-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cc795-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc795-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="cc795-126">Request body</span></span>
<span data-ttu-id="cc795-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="cc795-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cc795-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc795-128">Response</span></span>
<span data-ttu-id="cc795-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="cc795-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cc795-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="cc795-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cc795-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="cc795-131">Request</span></span>
<span data-ttu-id="cc795-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="cc795-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/userStatuses/{managedDeviceMobileAppConfigurationUserStatusId}
```

### <a name="response"></a><span data-ttu-id="cc795-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="cc795-133">Response</span></span>
<span data-ttu-id="cc795-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="cc795-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






