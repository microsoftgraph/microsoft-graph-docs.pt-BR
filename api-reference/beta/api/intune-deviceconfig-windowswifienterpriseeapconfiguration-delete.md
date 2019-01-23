---
title: Excluir windowsWifiEnterpriseEAPConfiguration
description: Exclui um windowsWifiEnterpriseEAPConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c04cefa6ec8e6f2b273871b9d4e8775b24a9fb14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29407400"
---
# <a name="delete-windowswifienterpriseeapconfiguration"></a><span data-ttu-id="9ac76-103">Excluir windowsWifiEnterpriseEAPConfiguration</span><span class="sxs-lookup"><span data-stu-id="9ac76-103">Delete windowsWifiEnterpriseEAPConfiguration</span></span>

> <span data-ttu-id="9ac76-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="9ac76-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="9ac76-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="9ac76-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9ac76-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="9ac76-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ac76-107">Exclui um [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="9ac76-107">Deletes a [windowsWifiEnterpriseEAPConfiguration](../resources/intune-deviceconfig-windowswifienterpriseeapconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ac76-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9ac76-108">Prerequisites</span></span>
<span data-ttu-id="9ac76-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="9ac76-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="9ac76-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9ac76-111">Permission type</span></span>|<span data-ttu-id="9ac76-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9ac76-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ac76-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9ac76-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ac76-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ac76-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9ac76-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9ac76-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ac76-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac76-116">Not supported.</span></span>|
|<span data-ttu-id="9ac76-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="9ac76-117">Application</span></span>|<span data-ttu-id="9ac76-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9ac76-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ac76-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9ac76-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="9ac76-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac76-120">Request headers</span></span>
|<span data-ttu-id="9ac76-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9ac76-121">Header</span></span>|<span data-ttu-id="9ac76-122">Valor</span><span class="sxs-lookup"><span data-stu-id="9ac76-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ac76-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="9ac76-123">Authorization</span></span>|<span data-ttu-id="9ac76-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9ac76-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ac76-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9ac76-125">Accept</span></span>|<span data-ttu-id="9ac76-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ac76-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ac76-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac76-127">Request body</span></span>
<span data-ttu-id="9ac76-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9ac76-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9ac76-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac76-129">Response</span></span>
<span data-ttu-id="9ac76-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9ac76-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9ac76-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9ac76-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ac76-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9ac76-132">Request</span></span>
<span data-ttu-id="9ac76-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9ac76-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="9ac76-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="9ac76-134">Response</span></span>
<span data-ttu-id="9ac76-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9ac76-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




