---
title: Visão geral da API de sincronização do Azure AD
description: ') permite que você automatize a criação, manutenção e remoção de identidades em nuvem aplicativos (software como um serviço ou SaaS) como a pasta de recados, a equipe de vendas, ServiceNow e muito mais. Você pode usar a APIs de sincronização no Microsoft Graph gerenciar a sincronização de identidade programaticamente, incluindo:'
ms.openlocfilehash: ff3acb00801c9b04b8257345b06100297e11710c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039790"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="06a19-104">Visão geral da API de sincronização do Azure AD</span><span class="sxs-lookup"><span data-stu-id="06a19-104">Azure AD synchronization API overview</span></span>

> <span data-ttu-id="06a19-105">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="06a19-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="06a19-106">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="06a19-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="06a19-107">Sincronização de identidades do Azure Active Directory (AD Azure) (também chamada de "provisionamento") permite automatizar a criação, manutenção e remoção de identidades em nuvem (software como um serviço ou SaaS) aplicativos, como a pasta de recados, a equipe de vendas, ServiceNow, e muito mais.</span><span class="sxs-lookup"><span data-stu-id="06a19-107">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="06a19-108">Você pode usar a APIs de sincronização no Microsoft Graph gerenciar a sincronização de identidade programaticamente, incluindo:</span><span class="sxs-lookup"><span data-stu-id="06a19-108">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="06a19-109">Criar, iniciar e interromper os trabalhos de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-109">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="06a19-110">Fazer alterações no esquema de sincronização para trabalhos</span><span class="sxs-lookup"><span data-stu-id="06a19-110">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="06a19-111">Verificar o status atual da sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-111">Verify the current synchronization status</span></span> 

<span data-ttu-id="06a19-112">Para obter mais informações sobre a sincronização do Azure AD, consulte:</span><span class="sxs-lookup"><span data-stu-id="06a19-112">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="06a19-113">Automatizar o usuário provisionamento e desprovisionamento SaaS aplicativos com o Windows Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="06a19-113">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="06a19-114">Gerenciando a conta de usuário de provisionamento para aplicativos de empresa no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="06a19-114">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="06a19-115">Você também pode tentar a API do [Explorer do gráfico](https://developer.microsoft.com/graph/graph-explorer) em um locatário de amostra ou seu próprio locatário.</span><span class="sxs-lookup"><span data-stu-id="06a19-115">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="06a19-116">Trabalho de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-116">Synchronization job</span></span>

<span data-ttu-id="06a19-117">Trabalhos de sincronização realizar a sincronização periodicamente em execução em segundo plano, sondagem para que as alterações em um diretório e envio-los para um diretório diferente.</span><span class="sxs-lookup"><span data-stu-id="06a19-117">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="06a19-118">O trabalho de sincronização sempre é específico para uma determinada instância de um aplicativo no seu locatário.</span><span class="sxs-lookup"><span data-stu-id="06a19-118">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="06a19-119">Como parte da configuração do trabalho de sincronização, você precisará fornecer a autorização para ler e gravar objetos em seu diretório de destino e personalize o esquema de sincronização de tarefa.</span><span class="sxs-lookup"><span data-stu-id="06a19-119">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="06a19-120">Para obter mais informações, consulte o [trabalho de sincronização](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="06a19-120">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="06a19-121">Esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-121">Synchronization schema</span></span>

<span data-ttu-id="06a19-122">O esquema de sincronização define quais objetos serão sincronizados e como eles serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="06a19-122">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="06a19-123">O esquema de sincronização contém a maioria das informações de instalação para um trabalho de sincronização específica.</span><span class="sxs-lookup"><span data-stu-id="06a19-123">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="06a19-124">Normalmente, você irá personalizar alguns dos [mapeamentos de atributo](synchronization-attributemapping.md)ou adicionar um [filtro de escopo](synchronization-filter.md) para sincronizar apenas os objetos que atender a uma determinada condição.</span><span class="sxs-lookup"><span data-stu-id="06a19-124">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="06a19-125">O esquema de sincronização inclui os seguintes componentes:</span><span class="sxs-lookup"><span data-stu-id="06a19-125">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="06a19-126">Definições do diretório</span><span class="sxs-lookup"><span data-stu-id="06a19-126">Directory definitions</span></span>
- <span data-ttu-id="06a19-127">Regras de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-127">Synchronization rules</span></span>
- <span data-ttu-id="06a19-128">Mapeamentos de objeto</span><span class="sxs-lookup"><span data-stu-id="06a19-128">Object mappings</span></span>

<span data-ttu-id="06a19-129">Para obter mais informações, consulte [esquema de sincronização](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="06a19-129">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="06a19-130">Modelo de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-130">Synchronization template</span></span>

<span data-ttu-id="06a19-131">O modelo de sincronização fornece configurações de sincronização pré-configurado para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="06a19-131">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="06a19-132">Essas configurações (o mais importante, o [esquema de sincronização](synchronization-synchronizationschema.md)) serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) que baseia-se no modelo.</span><span class="sxs-lookup"><span data-stu-id="06a19-132">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="06a19-133">Modelos são especificados pelo desenvolvedor de aplicativos.</span><span class="sxs-lookup"><span data-stu-id="06a19-133">Templates are specified by the application developer.</span></span>

<span data-ttu-id="06a19-134">Para obter mais informações, consulte [modelo de sincronização](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="06a19-134">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="06a19-135">Trabalhando com a API de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-135">Working with the synchronization API</span></span>

<span data-ttu-id="06a19-136">Trabalhando com a sincronização de API envolve principalmente a acessar os recursos [synchronizationJob](synchronization-synchronizationjob.md) e [synchronizationSchema](synchronization-synchronizationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="06a19-136">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="06a19-137">Para localizar seu recurso [synchronizationJob](synchronization-synchronizationjob.md) , você precisa saber a ID do objeto principal do serviço que pertence o trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="06a19-137">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="06a19-138">Os exemplos a seguir mostram como trabalhar com os recursos **synchronizationJob** e **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="06a19-138">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="06a19-139">Autorização</span><span class="sxs-lookup"><span data-stu-id="06a19-139">Authorization</span></span>

<span data-ttu-id="06a19-140">A API de sincronização do Azure AD usa OAuth 2.0 para autorização.</span><span class="sxs-lookup"><span data-stu-id="06a19-140">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="06a19-141">Antes de fazer quaisquer solicitações da API, você precisa obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="06a19-141">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="06a19-142">Para obter mais informações, consulte [tokens de acesso de Get para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="06a19-142">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="06a19-143">Para acessar os recursos de sincronização, seu aplicativo deve Directory.ReadWrite.All permissões.</span><span class="sxs-lookup"><span data-stu-id="06a19-143">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="06a19-144">Para obter mais informações, consulte [permissões de diretório](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="06a19-144">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="06a19-145">Localizar o objeto de entidade de serviço por nome para exibição</span><span class="sxs-lookup"><span data-stu-id="06a19-145">Find the service principal object by display name</span></span>

<span data-ttu-id="06a19-146">O exemplo a seguir mostra como localizar o objeto de entidade de serviço por nome para exibição.</span><span class="sxs-lookup"><span data-stu-id="06a19-146">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="06a19-147">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="06a19-147">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="06a19-148">**Response**</span><span class="sxs-lookup"><span data-stu-id="06a19-148">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="06a19-149">Localizar o objeto de entidade de serviço por ID de aplicativo</span><span class="sxs-lookup"><span data-stu-id="06a19-149">Find the service principal object by app ID</span></span>

<span data-ttu-id="06a19-150">O exemplo a seguir mostra como localizar o objeto de entidade de serviço por ID de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="06a19-150">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="06a19-151">**Solicitação** 
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-151">**Request** 
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="06a19-152">**Resposta**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-152">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="06a19-153">Listar os trabalhos de sincronização existente</span><span class="sxs-lookup"><span data-stu-id="06a19-153">List existing synchronization jobs</span></span>

<span data-ttu-id="06a19-154">O exemplo a seguir mostra como listar os trabalhos de sincronização existente.</span><span class="sxs-lookup"><span data-stu-id="06a19-154">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="06a19-155">**Solicitação**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-155">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="06a19-156">**Resposta**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-156">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="06a19-157">Obter o status do trabalho de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-157">Get synchronization job status</span></span>
<span data-ttu-id="06a19-158">O exemplo a seguir mostra como obter o status de um trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="06a19-158">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="06a19-159">**Solicitação**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-159">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="06a19-160">**Resposta**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-160">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="06a19-161">Obter o esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="06a19-161">Get synchronization schema</span></span>
<span data-ttu-id="06a19-162">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="06a19-162">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="06a19-163">**Solicitação**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-163">**Request**
<!-- { "blockType": "ignored" } --></span></span>
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="06a19-164">**Resposta**
<!-- { "blockType": "ignored" } --></span><span class="sxs-lookup"><span data-stu-id="06a19-164">**Response**
<!-- { "blockType": "ignored" } --></span></span>
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="06a19-165">Confira também</span><span class="sxs-lookup"><span data-stu-id="06a19-165">See also</span></span>

* [<span data-ttu-id="06a19-166">Configurar a sincronização com os atributos de extensão de diretório</span><span class="sxs-lookup"><span data-stu-id="06a19-166">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="06a19-167">Configurar a sincronização com atributos personalizados de destino</span><span class="sxs-lookup"><span data-stu-id="06a19-167">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



