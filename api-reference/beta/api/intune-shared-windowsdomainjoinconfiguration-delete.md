---
title: Excluir windowsDomainJoinConfiguration
description: Exclui um windowsDomainJoinConfiguration.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 04ef2c85351614533e21a107e8e1cbf9636bd753
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27821717"
---
# <a name="delete-windowsdomainjoinconfiguration"></a><span data-ttu-id="41b4b-103">Excluir windowsDomainJoinConfiguration</span><span class="sxs-lookup"><span data-stu-id="41b4b-103">Delete windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="41b4b-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="41b4b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="41b4b-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="41b4b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="41b4b-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="41b4b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="41b4b-107">Exclui um [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="41b4b-107">Deletes a [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="41b4b-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="41b4b-108">Prerequisites</span></span>
<span data-ttu-id="41b4b-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="41b4b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41b4b-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="41b4b-111">Permission type</span></span>|<span data-ttu-id="41b4b-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="41b4b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41b4b-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="41b4b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="41b4b-114">&nbsp; &nbsp; **Configuração do dispositivo**</span><span class="sxs-lookup"><span data-stu-id="41b4b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="41b4b-115">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41b4b-115">DeviceManagementConfiguration.ReadWrite.All</span></span> |
|<span data-ttu-id="41b4b-116">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="41b4b-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41b4b-117">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41b4b-117">Not supported.</span></span>|
|<span data-ttu-id="41b4b-118">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="41b4b-118">Application</span></span>|<span data-ttu-id="41b4b-119">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="41b4b-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41b4b-120">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="41b4b-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="41b4b-121">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="41b4b-121">Request headers</span></span>
|<span data-ttu-id="41b4b-122">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="41b4b-122">Header</span></span>|<span data-ttu-id="41b4b-123">Valor</span><span class="sxs-lookup"><span data-stu-id="41b4b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41b4b-124">Autorização</span><span class="sxs-lookup"><span data-stu-id="41b4b-124">Authorization</span></span>|<span data-ttu-id="41b4b-125">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="41b4b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41b4b-126">Aceitar</span><span class="sxs-lookup"><span data-stu-id="41b4b-126">Accept</span></span>|<span data-ttu-id="41b4b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="41b4b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41b4b-128">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="41b4b-128">Request body</span></span>
<span data-ttu-id="41b4b-129">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="41b4b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41b4b-130">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b4b-130">Response</span></span>
<span data-ttu-id="41b4b-131">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="41b4b-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="41b4b-132">Exemplo</span><span class="sxs-lookup"><span data-stu-id="41b4b-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="41b4b-133">Solicitação</span><span class="sxs-lookup"><span data-stu-id="41b4b-133">Request</span></span>
<span data-ttu-id="41b4b-134">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="41b4b-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="41b4b-135">Resposta</span><span class="sxs-lookup"><span data-stu-id="41b4b-135">Response</span></span>
<span data-ttu-id="41b4b-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="41b4b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



