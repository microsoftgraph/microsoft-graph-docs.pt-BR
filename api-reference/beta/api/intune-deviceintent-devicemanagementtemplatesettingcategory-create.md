---
title: Criar deviceManagementTemplateSettingCategory
description: Criar um novo objeto deviceManagementTemplateSettingCategory.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 903a39fd2e5b18742027f583a96e5d69b2d6986f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42814964"
---
# <a name="create-devicemanagementtemplatesettingcategory"></a><span data-ttu-id="1ba2a-103">Criar deviceManagementTemplateSettingCategory</span><span class="sxs-lookup"><span data-stu-id="1ba2a-103">Create deviceManagementTemplateSettingCategory</span></span>

> <span data-ttu-id="1ba2a-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1ba2a-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1ba2a-106">Criar um novo objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="1ba2a-106">Create a new [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1ba2a-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="1ba2a-107">Prerequisites</span></span>
<span data-ttu-id="1ba2a-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="1ba2a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1ba2a-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="1ba2a-110">Permission type</span></span>|<span data-ttu-id="1ba2a-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="1ba2a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1ba2a-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="1ba2a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1ba2a-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba2a-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="1ba2a-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="1ba2a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1ba2a-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-115">Not supported.</span></span>|
|<span data-ttu-id="1ba2a-116">Application</span><span class="sxs-lookup"><span data-stu-id="1ba2a-116">Application</span></span>|<span data-ttu-id="1ba2a-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1ba2a-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1ba2a-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="1ba2a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/templates/{deviceManagementTemplateId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="1ba2a-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="1ba2a-119">Request headers</span></span>
|<span data-ttu-id="1ba2a-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="1ba2a-120">Header</span></span>|<span data-ttu-id="1ba2a-121">Valor</span><span class="sxs-lookup"><span data-stu-id="1ba2a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1ba2a-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="1ba2a-122">Authorization</span></span>|<span data-ttu-id="1ba2a-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1ba2a-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="1ba2a-124">Accept</span></span>|<span data-ttu-id="1ba2a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1ba2a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1ba2a-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="1ba2a-126">Request body</span></span>
<span data-ttu-id="1ba2a-127">No corpo da solicitação, forneça uma representação JSON do objeto deviceManagementTemplateSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-127">In the request body, supply a JSON representation for the deviceManagementTemplateSettingCategory object.</span></span>

<span data-ttu-id="1ba2a-128">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceManagementTemplateSettingCategory.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-128">The following table shows the properties that are required when you create the deviceManagementTemplateSettingCategory.</span></span>

|<span data-ttu-id="1ba2a-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1ba2a-129">Property</span></span>|<span data-ttu-id="1ba2a-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="1ba2a-130">Type</span></span>|<span data-ttu-id="1ba2a-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="1ba2a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1ba2a-132">id</span><span class="sxs-lookup"><span data-stu-id="1ba2a-132">id</span></span>|<span data-ttu-id="1ba2a-133">String</span><span class="sxs-lookup"><span data-stu-id="1ba2a-133">String</span></span>|<span data-ttu-id="1ba2a-134">A ID de categoria herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1ba2a-134">The category ID Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="1ba2a-135">displayName</span><span class="sxs-lookup"><span data-stu-id="1ba2a-135">displayName</span></span>|<span data-ttu-id="1ba2a-136">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1ba2a-136">String</span></span>|<span data-ttu-id="1ba2a-137">O nome da categoria herdado de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1ba2a-137">The category name Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|
|<span data-ttu-id="1ba2a-138">hasRequiredSetting</span><span class="sxs-lookup"><span data-stu-id="1ba2a-138">hasRequiredSetting</span></span>|<span data-ttu-id="1ba2a-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="1ba2a-139">Boolean</span></span>|<span data-ttu-id="1ba2a-140">A categoria contém a configuração necessária de nível superior herdada de [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span><span class="sxs-lookup"><span data-stu-id="1ba2a-140">The category contains top level required setting Inherited from [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1ba2a-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ba2a-141">Response</span></span>
<span data-ttu-id="1ba2a-142">Se tiver êxito, este método retornará `201 Created` um código de resposta e um objeto [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-142">If successful, this method returns a `201 Created` response code and a [deviceManagementTemplateSettingCategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1ba2a-143">Exemplo</span><span class="sxs-lookup"><span data-stu-id="1ba2a-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="1ba2a-144">Solicitação</span><span class="sxs-lookup"><span data-stu-id="1ba2a-144">Request</span></span>
<span data-ttu-id="1ba2a-145">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/categories
Content-type: application/json
Content-length: 152

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```

### <a name="response"></a><span data-ttu-id="1ba2a-146">Resposta</span><span class="sxs-lookup"><span data-stu-id="1ba2a-146">Response</span></span>
<span data-ttu-id="1ba2a-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="1ba2a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 201

{
  "@odata.type": "#microsoft.graph.deviceManagementTemplateSettingCategory",
  "id": "cd213562-3562-cd21-6235-21cd623521cd",
  "displayName": "Display Name value",
  "hasRequiredSetting": true
}
```




