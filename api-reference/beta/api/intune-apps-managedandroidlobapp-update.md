---
title: Atualizar managedAndroidLobApp
description: Atualiza as propriedades de um objeto managedAndroidLobApp.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7baaccbb28702cbf71226a95ff7523763a007e87
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985715"
---
# <a name="update-managedandroidlobapp"></a><span data-ttu-id="f4866-103">Atualizar managedAndroidLobApp</span><span class="sxs-lookup"><span data-stu-id="f4866-103">Update managedAndroidLobApp</span></span>

> <span data-ttu-id="f4866-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f4866-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f4866-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f4866-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f4866-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f4866-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4866-107">Atualiza as propriedades de um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f4866-107">Update the properties of a [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4866-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f4866-108">Prerequisites</span></span>
<span data-ttu-id="f4866-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f4866-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4866-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f4866-111">Permission type</span></span>|<span data-ttu-id="f4866-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f4866-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4866-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f4866-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f4866-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4866-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f4866-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f4866-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4866-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4866-116">Not supported.</span></span>|
|<span data-ttu-id="f4866-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f4866-117">Application</span></span>|<span data-ttu-id="f4866-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f4866-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4866-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f4866-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f4866-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f4866-120">Request headers</span></span>
|<span data-ttu-id="f4866-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f4866-121">Header</span></span>|<span data-ttu-id="f4866-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f4866-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4866-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f4866-123">Authorization</span></span>|<span data-ttu-id="f4866-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f4866-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4866-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f4866-125">Accept</span></span>|<span data-ttu-id="f4866-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4866-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4866-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f4866-127">Request body</span></span>
<span data-ttu-id="f4866-128">No corpo da solicitação, forneça uma representação JSON do objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f4866-128">In the request body, supply a JSON representation for the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object.</span></span>

<span data-ttu-id="f4866-129">A tabela a seguir mostra as propriedades obrigatórias ao criar [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span><span class="sxs-lookup"><span data-stu-id="f4866-129">The following table shows the properties that are required when you create the [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md).</span></span>

|<span data-ttu-id="f4866-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f4866-130">Property</span></span>|<span data-ttu-id="f4866-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f4866-131">Type</span></span>|<span data-ttu-id="f4866-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f4866-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f4866-133">id</span><span class="sxs-lookup"><span data-stu-id="f4866-133">id</span></span>|<span data-ttu-id="f4866-134">String</span><span class="sxs-lookup"><span data-stu-id="f4866-134">String</span></span>|<span data-ttu-id="f4866-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f4866-135">Key of the entity.</span></span> <span data-ttu-id="f4866-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f4866-137">displayName</span></span>|<span data-ttu-id="f4866-138">String</span><span class="sxs-lookup"><span data-stu-id="f4866-138">String</span></span>|<span data-ttu-id="f4866-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f4866-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f4866-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-141">description</span><span class="sxs-lookup"><span data-stu-id="f4866-141">description</span></span>|<span data-ttu-id="f4866-142">String</span><span class="sxs-lookup"><span data-stu-id="f4866-142">String</span></span>|<span data-ttu-id="f4866-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-143">The description of the app.</span></span> <span data-ttu-id="f4866-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f4866-145">publisher</span></span>|<span data-ttu-id="f4866-146">String</span><span class="sxs-lookup"><span data-stu-id="f4866-146">String</span></span>|<span data-ttu-id="f4866-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-147">The publisher of the app.</span></span> <span data-ttu-id="f4866-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f4866-149">largeIcon</span></span>|[<span data-ttu-id="f4866-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f4866-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f4866-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f4866-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f4866-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4866-153">createdDateTime</span></span>|<span data-ttu-id="f4866-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4866-154">DateTimeOffset</span></span>|<span data-ttu-id="f4866-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-155">The date and time the app was created.</span></span> <span data-ttu-id="f4866-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4866-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f4866-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4866-158">DateTimeOffset</span></span>|<span data-ttu-id="f4866-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f4866-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f4866-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f4866-161">isFeatured</span></span>|<span data-ttu-id="f4866-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="f4866-162">Boolean</span></span>|<span data-ttu-id="f4866-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f4866-164">privacyInformationUrl</span></span>|<span data-ttu-id="f4866-165">String</span><span class="sxs-lookup"><span data-stu-id="f4866-165">String</span></span>|<span data-ttu-id="f4866-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f4866-166">The privacy statement Url.</span></span> <span data-ttu-id="f4866-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f4866-168">informationUrl</span></span>|<span data-ttu-id="f4866-169">String</span><span class="sxs-lookup"><span data-stu-id="f4866-169">String</span></span>|<span data-ttu-id="f4866-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f4866-170">The more information Url.</span></span> <span data-ttu-id="f4866-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-172">owner</span><span class="sxs-lookup"><span data-stu-id="f4866-172">owner</span></span>|<span data-ttu-id="f4866-173">String</span><span class="sxs-lookup"><span data-stu-id="f4866-173">String</span></span>|<span data-ttu-id="f4866-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f4866-174">The owner of the app.</span></span> <span data-ttu-id="f4866-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-176">developer</span><span class="sxs-lookup"><span data-stu-id="f4866-176">developer</span></span>|<span data-ttu-id="f4866-177">String</span><span class="sxs-lookup"><span data-stu-id="f4866-177">String</span></span>|<span data-ttu-id="f4866-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-178">The developer of the app.</span></span> <span data-ttu-id="f4866-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-180">Observações</span><span class="sxs-lookup"><span data-stu-id="f4866-180">notes</span></span>|<span data-ttu-id="f4866-181">String</span><span class="sxs-lookup"><span data-stu-id="f4866-181">String</span></span>|<span data-ttu-id="f4866-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-182">Notes for the app.</span></span> <span data-ttu-id="f4866-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f4866-184">uploadState</span></span>|<span data-ttu-id="f4866-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f4866-185">Int32</span></span>|<span data-ttu-id="f4866-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f4866-186">The upload state.</span></span> <span data-ttu-id="f4866-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f4866-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f4866-188">publishingState</span></span>|[<span data-ttu-id="f4866-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f4866-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f4866-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-190">The publishing state for the app.</span></span> <span data-ttu-id="f4866-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f4866-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f4866-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f4866-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f4866-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f4866-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f4866-194">appAvailability</span><span class="sxs-lookup"><span data-stu-id="f4866-194">appAvailability</span></span>|[<span data-ttu-id="f4866-195">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="f4866-195">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="f4866-196">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-196">The Application's availability.</span></span> <span data-ttu-id="f4866-197">Herdada do [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="f4866-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="f4866-198">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="f4866-198">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="f4866-199">version</span><span class="sxs-lookup"><span data-stu-id="f4866-199">version</span></span>|<span data-ttu-id="f4866-200">String</span><span class="sxs-lookup"><span data-stu-id="f4866-200">String</span></span>|<span data-ttu-id="f4866-201">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f4866-201">The Application's version.</span></span> <span data-ttu-id="f4866-202">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-202">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="f4866-203">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f4866-203">committedContentVersion</span></span>|<span data-ttu-id="f4866-204">String</span><span class="sxs-lookup"><span data-stu-id="f4866-204">String</span></span>|<span data-ttu-id="f4866-205">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f4866-205">The internal committed content version.</span></span> <span data-ttu-id="f4866-206">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-206">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f4866-207">fileName</span><span class="sxs-lookup"><span data-stu-id="f4866-207">fileName</span></span>|<span data-ttu-id="f4866-208">String</span><span class="sxs-lookup"><span data-stu-id="f4866-208">String</span></span>|<span data-ttu-id="f4866-209">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f4866-209">The name of the main Lob application file.</span></span> <span data-ttu-id="f4866-210">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-210">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f4866-211">size</span><span class="sxs-lookup"><span data-stu-id="f4866-211">size</span></span>|<span data-ttu-id="f4866-212">Int64</span><span class="sxs-lookup"><span data-stu-id="f4866-212">Int64</span></span>|<span data-ttu-id="f4866-213">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f4866-213">The total size, including all uploaded files.</span></span> <span data-ttu-id="f4866-214">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f4866-214">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="f4866-215">packageId</span><span class="sxs-lookup"><span data-stu-id="f4866-215">packageId</span></span>|<span data-ttu-id="f4866-216">String</span><span class="sxs-lookup"><span data-stu-id="f4866-216">String</span></span>|<span data-ttu-id="f4866-217">O identificador do pacote.</span><span class="sxs-lookup"><span data-stu-id="f4866-217">The package identifier.</span></span>|
|<span data-ttu-id="f4866-218">identityName</span><span class="sxs-lookup"><span data-stu-id="f4866-218">identityName</span></span>|<span data-ttu-id="f4866-219">String</span><span class="sxs-lookup"><span data-stu-id="f4866-219">String</span></span>|<span data-ttu-id="f4866-220">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="f4866-220">The Identity Name.</span></span>|
|<span data-ttu-id="f4866-221">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f4866-221">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f4866-222">androidMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f4866-222">androidMinimumOperatingSystem</span></span>](../resources/intune-apps-androidminimumoperatingsystem.md)|<span data-ttu-id="f4866-223">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f4866-223">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f4866-224">versionName</span><span class="sxs-lookup"><span data-stu-id="f4866-224">versionName</span></span>|<span data-ttu-id="f4866-225">String</span><span class="sxs-lookup"><span data-stu-id="f4866-225">String</span></span>|<span data-ttu-id="f4866-226">O nome da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f4866-226">The version name of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f4866-227">versionCode</span><span class="sxs-lookup"><span data-stu-id="f4866-227">versionCode</span></span>|<span data-ttu-id="f4866-228">String</span><span class="sxs-lookup"><span data-stu-id="f4866-228">String</span></span>|<span data-ttu-id="f4866-229">O código da versão do aplicativo gerenciado de Linha de Negócios (LoB) Android gerenciado.</span><span class="sxs-lookup"><span data-stu-id="f4866-229">The version code of managed Android Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="f4866-230">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f4866-230">identityVersion</span></span>|<span data-ttu-id="f4866-231">String</span><span class="sxs-lookup"><span data-stu-id="f4866-231">String</span></span>|<span data-ttu-id="f4866-232">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f4866-232">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f4866-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4866-233">Response</span></span>
<span data-ttu-id="f4866-234">Se tiver êxito, este método retornará o código de resposta `200 OK` e um objeto [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f4866-234">If successful, this method returns a `200 OK` response code and an updated [managedAndroidLobApp](../resources/intune-apps-managedandroidlobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4866-235">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f4866-235">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4866-236">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f4866-236">Request</span></span>
<span data-ttu-id="f4866-237">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f4866-237">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1384

{
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "uploadState": 11,
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f4866-238">Resposta</span><span class="sxs-lookup"><span data-stu-id="f4866-238">Response</span></span>
<span data-ttu-id="f4866-p122">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f4866-p122">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1551

{
  "@odata.type": "#microsoft.graph.managedAndroidLobApp",
  "id": "802b7ed3-7ed3-802b-d37e-2b80d37e2b80",
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
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "packageId": "Package Id value",
  "identityName": "Identity Name value",
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
    "v4_0": true,
    "v4_0_3": true,
    "v4_1": true,
    "v4_2": true,
    "v4_3": true,
    "v4_4": true,
    "v5_0": true,
    "v5_1": true,
    "v6_0": true,
    "v7_0": true,
    "v7_1": true,
    "v8_0": true,
    "v8_1": true,
    "v9_0": true
  },
  "versionName": "Version Name value",
  "versionCode": "Version Code value",
  "identityVersion": "Identity Version value"
}
```





