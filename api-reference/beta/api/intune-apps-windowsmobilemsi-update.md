---
title: Atualizar windowsMobileMSI
description: Atualiza as propriedades de um objeto windowsMobileMSI.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c1683bff6d0212deff060193aa624f56143246e
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409094"
---
# <a name="update-windowsmobilemsi"></a><span data-ttu-id="5a2d2-103">Atualizar windowsMobileMSI</span><span class="sxs-lookup"><span data-stu-id="5a2d2-103">Update windowsMobileMSI</span></span>

> <span data-ttu-id="5a2d2-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5a2d2-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5a2d2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5a2d2-107">Atualiza as propriedades de um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="5a2d2-107">Update the properties of a [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5a2d2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="5a2d2-108">Prerequisites</span></span>
<span data-ttu-id="5a2d2-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="5a2d2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5a2d2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="5a2d2-111">Permission type</span></span>|<span data-ttu-id="5a2d2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a2d2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5a2d2-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a2d2-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5a2d2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a2d2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-116">Not supported.</span></span>|
|<span data-ttu-id="5a2d2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="5a2d2-117">Application</span></span>|<span data-ttu-id="5a2d2-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a2d2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="5a2d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="5a2d2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2d2-120">Request headers</span></span>
|<span data-ttu-id="5a2d2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="5a2d2-121">Header</span></span>|<span data-ttu-id="5a2d2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="5a2d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a2d2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="5a2d2-123">Authorization</span></span>|<span data-ttu-id="5a2d2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a2d2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="5a2d2-125">Accept</span></span>|<span data-ttu-id="5a2d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5a2d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a2d2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2d2-127">Request body</span></span>
<span data-ttu-id="5a2d2-128">No corpo da solicitação, forneça uma representação JSON para o objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="5a2d2-128">In the request body, supply a JSON representation for the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object.</span></span>

<span data-ttu-id="5a2d2-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span><span class="sxs-lookup"><span data-stu-id="5a2d2-129">The following table shows the properties that are required when you create the [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md).</span></span>

|<span data-ttu-id="5a2d2-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5a2d2-130">Property</span></span>|<span data-ttu-id="5a2d2-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="5a2d2-131">Type</span></span>|<span data-ttu-id="5a2d2-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="5a2d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a2d2-133">id</span><span class="sxs-lookup"><span data-stu-id="5a2d2-133">id</span></span>|<span data-ttu-id="5a2d2-134">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-134">String</span></span>|<span data-ttu-id="5a2d2-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-135">Key of the entity.</span></span> <span data-ttu-id="5a2d2-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-137">displayName</span><span class="sxs-lookup"><span data-stu-id="5a2d2-137">displayName</span></span>|<span data-ttu-id="5a2d2-138">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-138">String</span></span>|<span data-ttu-id="5a2d2-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="5a2d2-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-141">description</span><span class="sxs-lookup"><span data-stu-id="5a2d2-141">description</span></span>|<span data-ttu-id="5a2d2-142">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-142">String</span></span>|<span data-ttu-id="5a2d2-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-143">The description of the app.</span></span> <span data-ttu-id="5a2d2-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-145">publisher</span><span class="sxs-lookup"><span data-stu-id="5a2d2-145">publisher</span></span>|<span data-ttu-id="5a2d2-146">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-146">String</span></span>|<span data-ttu-id="5a2d2-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-147">The publisher of the app.</span></span> <span data-ttu-id="5a2d2-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="5a2d2-149">largeIcon</span></span>|[<span data-ttu-id="5a2d2-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5a2d2-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="5a2d2-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="5a2d2-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a2d2-153">createdDateTime</span></span>|<span data-ttu-id="5a2d2-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a2d2-154">DateTimeOffset</span></span>|<span data-ttu-id="5a2d2-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-155">The date and time the app was created.</span></span> <span data-ttu-id="5a2d2-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a2d2-157">lastModifiedDateTime</span></span>|<span data-ttu-id="5a2d2-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a2d2-158">DateTimeOffset</span></span>|<span data-ttu-id="5a2d2-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-159">The date and time the app was last modified.</span></span> <span data-ttu-id="5a2d2-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="5a2d2-161">isFeatured</span></span>|<span data-ttu-id="5a2d2-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a2d2-162">Boolean</span></span>|<span data-ttu-id="5a2d2-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="5a2d2-164">privacyInformationUrl</span></span>|<span data-ttu-id="5a2d2-165">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-165">String</span></span>|<span data-ttu-id="5a2d2-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-166">The privacy statement Url.</span></span> <span data-ttu-id="5a2d2-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="5a2d2-168">informationUrl</span></span>|<span data-ttu-id="5a2d2-169">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-169">String</span></span>|<span data-ttu-id="5a2d2-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-170">The more information Url.</span></span> <span data-ttu-id="5a2d2-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-172">owner</span><span class="sxs-lookup"><span data-stu-id="5a2d2-172">owner</span></span>|<span data-ttu-id="5a2d2-173">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-173">String</span></span>|<span data-ttu-id="5a2d2-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-174">The owner of the app.</span></span> <span data-ttu-id="5a2d2-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-176">developer</span><span class="sxs-lookup"><span data-stu-id="5a2d2-176">developer</span></span>|<span data-ttu-id="5a2d2-177">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-177">String</span></span>|<span data-ttu-id="5a2d2-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-178">The developer of the app.</span></span> <span data-ttu-id="5a2d2-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-180">Observações</span><span class="sxs-lookup"><span data-stu-id="5a2d2-180">notes</span></span>|<span data-ttu-id="5a2d2-181">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-181">String</span></span>|<span data-ttu-id="5a2d2-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-182">Notes for the app.</span></span> <span data-ttu-id="5a2d2-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="5a2d2-184">uploadState</span></span>|<span data-ttu-id="5a2d2-185">Int32</span><span class="sxs-lookup"><span data-stu-id="5a2d2-185">Int32</span></span>|<span data-ttu-id="5a2d2-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-186">The upload state.</span></span> <span data-ttu-id="5a2d2-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="5a2d2-188">publishingState</span></span>|[<span data-ttu-id="5a2d2-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="5a2d2-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="5a2d2-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-190">The publishing state for the app.</span></span> <span data-ttu-id="5a2d2-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="5a2d2-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="5a2d2-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="5a2d2-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="5a2d2-194">isAssigned</span><span class="sxs-lookup"><span data-stu-id="5a2d2-194">isAssigned</span></span>|<span data-ttu-id="5a2d2-195">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a2d2-195">Boolean</span></span>|<span data-ttu-id="5a2d2-196">O valor que indica se o aplicativo é atribuído a pelo menos um grupo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-196">The value indicating whether the app is assigned to at least one group.</span></span> <span data-ttu-id="5a2d2-197">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-197">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-198">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="5a2d2-198">roleScopeTagIds</span></span>|<span data-ttu-id="5a2d2-199">String collection</span><span class="sxs-lookup"><span data-stu-id="5a2d2-199">String collection</span></span>|<span data-ttu-id="5a2d2-200">Lista de ids de marca de escopo para esse aplicativo móvel.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-200">List of scope tag ids for this mobile app.</span></span> <span data-ttu-id="5a2d2-201">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-201">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="5a2d2-202">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="5a2d2-202">committedContentVersion</span></span>|<span data-ttu-id="5a2d2-203">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-203">String</span></span>|<span data-ttu-id="5a2d2-204">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-204">The internal committed content version.</span></span> <span data-ttu-id="5a2d2-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5a2d2-206">fileName</span><span class="sxs-lookup"><span data-stu-id="5a2d2-206">fileName</span></span>|<span data-ttu-id="5a2d2-207">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-207">String</span></span>|<span data-ttu-id="5a2d2-208">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-208">The name of the main Lob application file.</span></span> <span data-ttu-id="5a2d2-209">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-209">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5a2d2-210">size</span><span class="sxs-lookup"><span data-stu-id="5a2d2-210">size</span></span>|<span data-ttu-id="5a2d2-211">Int64</span><span class="sxs-lookup"><span data-stu-id="5a2d2-211">Int64</span></span>|<span data-ttu-id="5a2d2-212">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-212">The total size, including all uploaded files.</span></span> <span data-ttu-id="5a2d2-213">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="5a2d2-213">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="5a2d2-214">commandLine</span><span class="sxs-lookup"><span data-stu-id="5a2d2-214">commandLine</span></span>|<span data-ttu-id="5a2d2-215">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-215">String</span></span>|<span data-ttu-id="5a2d2-216">A linha de comando.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-216">The command line.</span></span>|
|<span data-ttu-id="5a2d2-217">productCode</span><span class="sxs-lookup"><span data-stu-id="5a2d2-217">productCode</span></span>|<span data-ttu-id="5a2d2-218">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-218">String</span></span>|<span data-ttu-id="5a2d2-219">O código do produto.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-219">The product code.</span></span>|
|<span data-ttu-id="5a2d2-220">productVersion</span><span class="sxs-lookup"><span data-stu-id="5a2d2-220">productVersion</span></span>|<span data-ttu-id="5a2d2-221">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-221">String</span></span>|<span data-ttu-id="5a2d2-222">A versão de produto do aplicativo de linha de negócios (LoB) Windows Mobile MSI.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-222">The product version of Windows Mobile MSI Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="5a2d2-223">ignoreVersionDetection</span><span class="sxs-lookup"><span data-stu-id="5a2d2-223">ignoreVersionDetection</span></span>|<span data-ttu-id="5a2d2-224">Boolean</span><span class="sxs-lookup"><span data-stu-id="5a2d2-224">Boolean</span></span>|<span data-ttu-id="5a2d2-225">Um booliano para controlar se a versão do aplicativo será usada para detectar o aplicativo depois que ele for instalado em um dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-225">A boolean to control whether the app's version will be used to detect the app after it is installed on a device.</span></span> <span data-ttu-id="5a2d2-226">Defina como true para o aplicativos de linha de negócios (LoB) Windows Mobile MSI que usam um recurso de atualização automática.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-226">Set this to true for Windows Mobile MSI Line of Business (LoB) apps that use a self update feature.</span></span>|
|<span data-ttu-id="5a2d2-227">identityVersion</span><span class="sxs-lookup"><span data-stu-id="5a2d2-227">identityVersion</span></span>|<span data-ttu-id="5a2d2-228">String</span><span class="sxs-lookup"><span data-stu-id="5a2d2-228">String</span></span>|<span data-ttu-id="5a2d2-229">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-229">The identity version.</span></span>|
|<span data-ttu-id="5a2d2-230">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="5a2d2-230">useDeviceContext</span></span>|<span data-ttu-id="5a2d2-231">Booliano</span><span class="sxs-lookup"><span data-stu-id="5a2d2-231">Boolean</span></span>|<span data-ttu-id="5a2d2-232">Indica se a instalação MSI um modo duplo no contexto do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-232">Indicates whether to install a dual-mode MSI in the device context.</span></span> <span data-ttu-id="5a2d2-233">Se for true, aplicativo será instalado para todos os usuários.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-233">If true, app will be installed for all users.</span></span> <span data-ttu-id="5a2d2-234">Se for false, o aplicativo será instalado por usuário.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-234">If false, app will be installed per-user.</span></span> <span data-ttu-id="5a2d2-235">Se for null, serviço usará o contexto de instalação do pacote MSI padrão.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-235">If null, service will use the MSI package's default install context.</span></span> <span data-ttu-id="5a2d2-236">Em caso de modo duplo MSI, esse padrão serão por usuário.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-236">In case of dual-mode MSI, this default will be per-user.</span></span>  <span data-ttu-id="5a2d2-237">Não podem ser definidas para aplicativos de modo não-duplo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-237">Cannot be set for non-dual-mode apps.</span></span>  <span data-ttu-id="5a2d2-238">Não pode ser alterada após a criação inicial do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-238">Cannot be changed after initial creation of the application.</span></span>|



## <a name="response"></a><span data-ttu-id="5a2d2-239">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a2d2-239">Response</span></span>
<span data-ttu-id="5a2d2-240">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-240">If successful, this method returns a `200 OK` response code and an updated [windowsMobileMSI](../resources/intune-apps-windowsmobilemsi.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a2d2-241">Exemplo</span><span class="sxs-lookup"><span data-stu-id="5a2d2-241">Example</span></span>

### <a name="request"></a><span data-ttu-id="5a2d2-242">Solicitação</span><span class="sxs-lookup"><span data-stu-id="5a2d2-242">Request</span></span>
<span data-ttu-id="5a2d2-243">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-243">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1039

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```

### <a name="response"></a><span data-ttu-id="5a2d2-244">Resposta</span><span class="sxs-lookup"><span data-stu-id="5a2d2-244">Response</span></span>
<span data-ttu-id="5a2d2-p124">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="5a2d2-p124">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1211

{
  "@odata.type": "#microsoft.graph.windowsMobileMSI",
  "id": "aa453e5d-3e5d-aa45-5d3e-45aa5d3e45aa",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "isAssigned": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "commandLine": "Command Line value",
  "productCode": "Product Code value",
  "productVersion": "Product Version value",
  "ignoreVersionDetection": true,
  "identityVersion": "Identity Version value",
  "useDeviceContext": true
}
```




