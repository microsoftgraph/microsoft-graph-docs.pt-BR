---
title: Listar androidForWorkAppConfigurationSchemas
description: Listar propriedades e relações dos objetos androidForWorkAppConfigurationSchema.
author: tfitzmac
ms.openlocfilehash: 140a49f8cbb93b6c1990dd80ee4eaec8e23c1859
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27358930"
---
# <a name="list-androidforworkappconfigurationschemas"></a><span data-ttu-id="6f2ef-103">Listar androidForWorkAppConfigurationSchemas</span><span class="sxs-lookup"><span data-stu-id="6f2ef-103">List androidForWorkAppConfigurationSchemas</span></span>

> <span data-ttu-id="6f2ef-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6f2ef-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6f2ef-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6f2ef-107">Listar propriedades e relações dos objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md).</span><span class="sxs-lookup"><span data-stu-id="6f2ef-107">List properties and relationships of the [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6f2ef-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6f2ef-108">Prerequisites</span></span>
<span data-ttu-id="6f2ef-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6f2ef-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f2ef-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6f2ef-111">Permission type</span></span>|<span data-ttu-id="6f2ef-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6f2ef-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f2ef-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6f2ef-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6f2ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f2ef-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f2ef-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6f2ef-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f2ef-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-116">Not supported.</span></span>|
|<span data-ttu-id="6f2ef-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6f2ef-117">Application</span></span>|<span data-ttu-id="6f2ef-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f2ef-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6f2ef-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkAppConfigurationSchemas
```

## <a name="request-headers"></a><span data-ttu-id="6f2ef-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2ef-120">Request headers</span></span>
|<span data-ttu-id="6f2ef-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6f2ef-121">Header</span></span>|<span data-ttu-id="6f2ef-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6f2ef-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f2ef-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6f2ef-123">Authorization</span></span>|<span data-ttu-id="6f2ef-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f2ef-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6f2ef-125">Accept</span></span>|<span data-ttu-id="6f2ef-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6f2ef-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f2ef-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2ef-127">Request body</span></span>
<span data-ttu-id="6f2ef-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f2ef-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f2ef-129">Response</span></span>
<span data-ttu-id="6f2ef-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkAppConfigurationSchema](../resources/intune-androidforwork-androidforworkappconfigurationschema.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f2ef-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6f2ef-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6f2ef-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6f2ef-132">Request</span></span>
<span data-ttu-id="6f2ef-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkAppConfigurationSchemas
```

### <a name="response"></a><span data-ttu-id="6f2ef-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="6f2ef-134">Response</span></span>
<span data-ttu-id="6f2ef-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6f2ef-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 977

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchema",
      "id": "c1230dc6-0dc6-c123-c60d-23c1c60d23c1",
      "exampleJson": "ZXhhbXBsZUpzb24=",
      "schemaItems": [
        {
          "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem",
          "schemaItemKey": "Schema Item Key value",
          "displayName": "Display Name value",
          "description": "Description value",
          "defaultBoolValue": true,
          "defaultIntValue": 15,
          "defaultStringValue": "Default String Value value",
          "defaultStringArrayValue": [
            "Default String Array Value value"
          ],
          "dataType": "integer",
          "selections": [
            {
              "@odata.type": "microsoft.graph.keyValuePair",
              "name": "Name value",
              "value": "Value value"
            }
          ]
        }
      ]
    }
  ]
}
```





