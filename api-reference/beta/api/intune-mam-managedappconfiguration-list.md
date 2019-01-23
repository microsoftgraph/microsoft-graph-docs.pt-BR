---
title: Listar managedAppConfigurations
description: Listar propriedades e relações dos objetos managedAppConfiguration.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5c35fa6e3c7da253675d247797c5f01605706478
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29423423"
---
# <a name="list-managedappconfigurations"></a><span data-ttu-id="7b5de-103">Listar managedAppConfigurations</span><span class="sxs-lookup"><span data-stu-id="7b5de-103">List managedAppConfigurations</span></span>

> <span data-ttu-id="7b5de-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7b5de-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7b5de-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7b5de-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7b5de-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7b5de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7b5de-107">Listar propriedades e relações dos objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="7b5de-107">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7b5de-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7b5de-108">Prerequisites</span></span>
<span data-ttu-id="7b5de-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7b5de-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7b5de-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7b5de-111">Permission type</span></span>|<span data-ttu-id="7b5de-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7b5de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7b5de-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7b5de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7b5de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="7b5de-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="7b5de-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7b5de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7b5de-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b5de-116">Not supported.</span></span>|
|<span data-ttu-id="7b5de-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7b5de-117">Application</span></span>|<span data-ttu-id="7b5de-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7b5de-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7b5de-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7b5de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/appliedPolicies
GET /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/intendedPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7b5de-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7b5de-120">Request headers</span></span>
|<span data-ttu-id="7b5de-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7b5de-121">Header</span></span>|<span data-ttu-id="7b5de-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7b5de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7b5de-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7b5de-123">Authorization</span></span>|<span data-ttu-id="7b5de-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7b5de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7b5de-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7b5de-125">Accept</span></span>|<span data-ttu-id="7b5de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7b5de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7b5de-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7b5de-127">Request body</span></span>
<span data-ttu-id="7b5de-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="7b5de-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7b5de-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b5de-129">Response</span></span>
<span data-ttu-id="7b5de-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7b5de-130">If successful, this method returns a `200 OK` response code and a collection of [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7b5de-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7b5de-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7b5de-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7b5de-132">Request</span></span>
<span data-ttu-id="7b5de-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7b5de-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppPolicies
```

### <a name="response"></a><span data-ttu-id="7b5de-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="7b5de-134">Response</span></span>
<span data-ttu-id="7b5de-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7b5de-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 666

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppConfiguration",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "2ed27cb5-7cb5-2ed2-b57c-d22eb57cd22e",
      "version": "Version value",
      "customSettings": [
        {
          "@odata.type": "microsoft.graph.keyValuePair",
          "name": "Name value",
          "value": "Value value"
        }
      ]
    }
  ]
}
```




