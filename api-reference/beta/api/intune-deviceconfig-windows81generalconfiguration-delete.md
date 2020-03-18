---
title: Excluir windows81GeneralConfiguration
description: Exclui windows81GeneralConfiguration
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac04cd6b14571c4004e3fa18c0e867c9eb79b491
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42737312"
---
# <a name="delete-windows81generalconfiguration"></a><span data-ttu-id="2bd45-103">Excluir windows81GeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="2bd45-103">Delete windows81GeneralConfiguration</span></span>

> <span data-ttu-id="2bd45-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="2bd45-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2bd45-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="2bd45-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2bd45-106">Exclui [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="2bd45-106">Deletes a [windows81GeneralConfiguration](../resources/intune-deviceconfig-windows81generalconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2bd45-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="2bd45-107">Prerequisites</span></span>
<span data-ttu-id="2bd45-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2bd45-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2bd45-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="2bd45-110">Permission type</span></span>|<span data-ttu-id="2bd45-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="2bd45-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2bd45-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="2bd45-112">Delegated (work or school account)</span></span>|<span data-ttu-id="2bd45-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bd45-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2bd45-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="2bd45-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2bd45-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="2bd45-115">Not supported.</span></span>|
|<span data-ttu-id="2bd45-116">Application</span><span class="sxs-lookup"><span data-stu-id="2bd45-116">Application</span></span>|<span data-ttu-id="2bd45-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2bd45-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2bd45-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="2bd45-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2bd45-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="2bd45-119">Request headers</span></span>
|<span data-ttu-id="2bd45-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="2bd45-120">Header</span></span>|<span data-ttu-id="2bd45-121">Valor</span><span class="sxs-lookup"><span data-stu-id="2bd45-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2bd45-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="2bd45-122">Authorization</span></span>|<span data-ttu-id="2bd45-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="2bd45-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2bd45-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="2bd45-124">Accept</span></span>|<span data-ttu-id="2bd45-125">application/json</span><span class="sxs-lookup"><span data-stu-id="2bd45-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2bd45-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="2bd45-126">Request body</span></span>
<span data-ttu-id="2bd45-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="2bd45-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2bd45-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bd45-128">Response</span></span>
<span data-ttu-id="2bd45-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="2bd45-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2bd45-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="2bd45-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="2bd45-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="2bd45-131">Request</span></span>
<span data-ttu-id="2bd45-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="2bd45-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2bd45-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="2bd45-133">Response</span></span>
<span data-ttu-id="2bd45-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="2bd45-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




