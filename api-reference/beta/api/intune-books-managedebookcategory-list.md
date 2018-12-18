---
title: Lista managedEBookCategories
description: Lista as propriedades e os relacionamentos dos objetos managedEBookCategory.
author: tfitzmac
ms.openlocfilehash: f4ffe260e1d6e66d981376cf0d5f96a22790a1f4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347730"
---
# <a name="list-managedebookcategories"></a><span data-ttu-id="387bf-103">Lista managedEBookCategories</span><span class="sxs-lookup"><span data-stu-id="387bf-103">List managedEBookCategories</span></span>

> <span data-ttu-id="387bf-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="387bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="387bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="387bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="387bf-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="387bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="387bf-107">Lista as propriedades e os relacionamentos dos objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) .</span><span class="sxs-lookup"><span data-stu-id="387bf-107">List properties and relationships of the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="387bf-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="387bf-108">Prerequisites</span></span>
<span data-ttu-id="387bf-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="387bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="387bf-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="387bf-111">Permission type</span></span>|<span data-ttu-id="387bf-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="387bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="387bf-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="387bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="387bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="387bf-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="387bf-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="387bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="387bf-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="387bf-116">Not supported.</span></span>|
|<span data-ttu-id="387bf-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="387bf-117">Application</span></span>|<span data-ttu-id="387bf-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="387bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="387bf-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="387bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBookCategories
GET /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="387bf-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="387bf-120">Request headers</span></span>
|<span data-ttu-id="387bf-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="387bf-121">Header</span></span>|<span data-ttu-id="387bf-122">Valor</span><span class="sxs-lookup"><span data-stu-id="387bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="387bf-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="387bf-123">Authorization</span></span>|<span data-ttu-id="387bf-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="387bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="387bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="387bf-125">Accept</span></span>|<span data-ttu-id="387bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="387bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="387bf-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="387bf-127">Request body</span></span>
<span data-ttu-id="387bf-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="387bf-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="387bf-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="387bf-129">Response</span></span>
<span data-ttu-id="387bf-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [managedEBookCategory](../resources/intune-books-managedebookcategory.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="387bf-130">If successful, this method returns a `200 OK` response code and a collection of [managedEBookCategory](../resources/intune-books-managedebookcategory.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="387bf-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="387bf-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="387bf-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="387bf-132">Request</span></span>
<span data-ttu-id="387bf-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="387bf-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
```

### <a name="response"></a><span data-ttu-id="387bf-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="387bf-134">Response</span></span>
<span data-ttu-id="387bf-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="387bf-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 264

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedEBookCategory",
      "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
      "displayName": "Display Name value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
    }
  ]
}
```





