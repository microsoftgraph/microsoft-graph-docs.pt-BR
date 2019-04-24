---
title: Excluir mobileAppProvisioningConfigGroupAssignment
description: Exclui mobileAppProvisioningConfigGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 328bad467a3c2f4923ca1076ca34530721724c9f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32488642"
---
# <a name="delete-mobileappprovisioningconfiggroupassignment"></a><span data-ttu-id="60d60-103">Excluir mobileAppProvisioningConfigGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="60d60-103">Delete mobileAppProvisioningConfigGroupAssignment</span></span>

> <span data-ttu-id="60d60-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="60d60-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60d60-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="60d60-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60d60-106">Exclui [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60d60-106">Deletes a [mobileAppProvisioningConfigGroupAssignment](../resources/intune-apps-mobileappprovisioningconfiggroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60d60-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60d60-107">Prerequisites</span></span>
<span data-ttu-id="60d60-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="60d60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60d60-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60d60-110">Permission type</span></span>|<span data-ttu-id="60d60-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60d60-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60d60-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60d60-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60d60-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60d60-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60d60-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60d60-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60d60-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60d60-115">Not supported.</span></span>|
|<span data-ttu-id="60d60-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60d60-116">Application</span></span>|<span data-ttu-id="60d60-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60d60-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60d60-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60d60-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="60d60-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60d60-119">Request headers</span></span>
|<span data-ttu-id="60d60-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60d60-120">Header</span></span>|<span data-ttu-id="60d60-121">Valor</span><span class="sxs-lookup"><span data-stu-id="60d60-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60d60-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="60d60-122">Authorization</span></span>|<span data-ttu-id="60d60-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60d60-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60d60-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60d60-124">Accept</span></span>|<span data-ttu-id="60d60-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60d60-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60d60-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60d60-126">Request body</span></span>
<span data-ttu-id="60d60-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60d60-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60d60-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="60d60-128">Response</span></span>
<span data-ttu-id="60d60-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60d60-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="60d60-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60d60-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60d60-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60d60-131">Request</span></span>
<span data-ttu-id="60d60-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60d60-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}/groupAssignments/{mobileAppProvisioningConfigGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="60d60-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="60d60-133">Response</span></span>
<span data-ttu-id="60d60-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60d60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





