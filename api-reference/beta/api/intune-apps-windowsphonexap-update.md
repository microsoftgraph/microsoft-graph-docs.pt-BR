---
title: Atualizar windowsPhoneXAP
description: Atualize as propriedades de um objeto windowsPhoneXAP.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 55bd6c3df68dbe76b0ce36e94f49e2a7c8d50f10
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27944331"
---
# <a name="update-windowsphonexap"></a><span data-ttu-id="f1f64-103">Atualizar windowsPhoneXAP</span><span class="sxs-lookup"><span data-stu-id="f1f64-103">Update windowsPhoneXAP</span></span>

> <span data-ttu-id="f1f64-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="f1f64-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f1f64-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="f1f64-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f1f64-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="f1f64-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f1f64-107">Atualize as propriedades de um objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="f1f64-107">Update the properties of a [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f1f64-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="f1f64-108">Prerequisites</span></span>
<span data-ttu-id="f1f64-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="f1f64-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f1f64-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="f1f64-111">Permission type</span></span>|<span data-ttu-id="f1f64-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="f1f64-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f1f64-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="f1f64-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f1f64-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f1f64-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f1f64-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="f1f64-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f1f64-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f64-116">Not supported.</span></span>|
|<span data-ttu-id="f1f64-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="f1f64-117">Application</span></span>|<span data-ttu-id="f1f64-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="f1f64-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f1f64-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="f1f64-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app
```

## <a name="request-headers"></a><span data-ttu-id="f1f64-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f64-120">Request headers</span></span>
|<span data-ttu-id="f1f64-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="f1f64-121">Header</span></span>|<span data-ttu-id="f1f64-122">Valor</span><span class="sxs-lookup"><span data-stu-id="f1f64-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f1f64-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="f1f64-123">Authorization</span></span>|<span data-ttu-id="f1f64-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="f1f64-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f1f64-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="f1f64-125">Accept</span></span>|<span data-ttu-id="f1f64-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f1f64-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f1f64-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f64-127">Request body</span></span>
<span data-ttu-id="f1f64-128">No corpo da solicitação, fornece uma representação JSON para o objeto [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) .</span><span class="sxs-lookup"><span data-stu-id="f1f64-128">In the request body, supply a JSON representation for the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object.</span></span>

<span data-ttu-id="f1f64-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span><span class="sxs-lookup"><span data-stu-id="f1f64-129">The following table shows the properties that are required when you create the [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md).</span></span>

|<span data-ttu-id="f1f64-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f1f64-130">Property</span></span>|<span data-ttu-id="f1f64-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="f1f64-131">Type</span></span>|<span data-ttu-id="f1f64-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="f1f64-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f1f64-133">id</span><span class="sxs-lookup"><span data-stu-id="f1f64-133">id</span></span>|<span data-ttu-id="f1f64-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-134">String</span></span>|<span data-ttu-id="f1f64-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="f1f64-135">Key of the entity.</span></span> <span data-ttu-id="f1f64-136">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-136">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f1f64-137">displayName</span></span>|<span data-ttu-id="f1f64-138">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-138">String</span></span>|<span data-ttu-id="f1f64-139">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="f1f64-139">The admin provided or imported title of the app.</span></span> <span data-ttu-id="f1f64-140">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-140">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-141">description</span><span class="sxs-lookup"><span data-stu-id="f1f64-141">description</span></span>|<span data-ttu-id="f1f64-142">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-142">String</span></span>|<span data-ttu-id="f1f64-143">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-143">The description of the app.</span></span> <span data-ttu-id="f1f64-144">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-144">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-145">publisher</span><span class="sxs-lookup"><span data-stu-id="f1f64-145">publisher</span></span>|<span data-ttu-id="f1f64-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-146">String</span></span>|<span data-ttu-id="f1f64-147">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-147">The publisher of the app.</span></span> <span data-ttu-id="f1f64-148">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-148">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-149">largeIcon</span><span class="sxs-lookup"><span data-stu-id="f1f64-149">largeIcon</span></span>|[<span data-ttu-id="f1f64-150">mimeContent</span><span class="sxs-lookup"><span data-stu-id="f1f64-150">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="f1f64-151">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="f1f64-151">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="f1f64-152">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-152">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-153">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f1f64-153">createdDateTime</span></span>|<span data-ttu-id="f1f64-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1f64-154">DateTimeOffset</span></span>|<span data-ttu-id="f1f64-155">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-155">The date and time the app was created.</span></span> <span data-ttu-id="f1f64-156">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-156">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-157">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f1f64-157">lastModifiedDateTime</span></span>|<span data-ttu-id="f1f64-158">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1f64-158">DateTimeOffset</span></span>|<span data-ttu-id="f1f64-159">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="f1f64-159">The date and time the app was last modified.</span></span> <span data-ttu-id="f1f64-160">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-160">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-161">isFeatured</span><span class="sxs-lookup"><span data-stu-id="f1f64-161">isFeatured</span></span>|<span data-ttu-id="f1f64-162">Booliano</span><span class="sxs-lookup"><span data-stu-id="f1f64-162">Boolean</span></span>|<span data-ttu-id="f1f64-163">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-163">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-164">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="f1f64-164">privacyInformationUrl</span></span>|<span data-ttu-id="f1f64-165">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-165">String</span></span>|<span data-ttu-id="f1f64-166">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="f1f64-166">The privacy statement Url.</span></span> <span data-ttu-id="f1f64-167">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-167">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-168">informationUrl</span><span class="sxs-lookup"><span data-stu-id="f1f64-168">informationUrl</span></span>|<span data-ttu-id="f1f64-169">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-169">String</span></span>|<span data-ttu-id="f1f64-170">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="f1f64-170">The more information Url.</span></span> <span data-ttu-id="f1f64-171">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-171">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-172">owner</span><span class="sxs-lookup"><span data-stu-id="f1f64-172">owner</span></span>|<span data-ttu-id="f1f64-173">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-173">String</span></span>|<span data-ttu-id="f1f64-174">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-174">The owner of the app.</span></span> <span data-ttu-id="f1f64-175">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-175">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-176">developer</span><span class="sxs-lookup"><span data-stu-id="f1f64-176">developer</span></span>|<span data-ttu-id="f1f64-177">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-177">String</span></span>|<span data-ttu-id="f1f64-178">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-178">The developer of the app.</span></span> <span data-ttu-id="f1f64-179">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-179">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-180">Observações</span><span class="sxs-lookup"><span data-stu-id="f1f64-180">notes</span></span>|<span data-ttu-id="f1f64-181">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-181">String</span></span>|<span data-ttu-id="f1f64-182">Anotações para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-182">Notes for the app.</span></span> <span data-ttu-id="f1f64-183">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-183">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-184">uploadState</span><span class="sxs-lookup"><span data-stu-id="f1f64-184">uploadState</span></span>|<span data-ttu-id="f1f64-185">Int32</span><span class="sxs-lookup"><span data-stu-id="f1f64-185">Int32</span></span>|<span data-ttu-id="f1f64-186">O estado de carregamento.</span><span class="sxs-lookup"><span data-stu-id="f1f64-186">The upload state.</span></span> <span data-ttu-id="f1f64-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="f1f64-188">publishingState</span><span class="sxs-lookup"><span data-stu-id="f1f64-188">publishingState</span></span>|[<span data-ttu-id="f1f64-189">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="f1f64-189">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="f1f64-190">O estado de publicação para o aplicativo.</span><span class="sxs-lookup"><span data-stu-id="f1f64-190">The publishing state for the app.</span></span> <span data-ttu-id="f1f64-191">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="f1f64-191">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="f1f64-192">Herdada do [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="f1f64-192">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="f1f64-193">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="f1f64-193">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="f1f64-194">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="f1f64-194">committedContentVersion</span></span>|<span data-ttu-id="f1f64-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-195">String</span></span>|<span data-ttu-id="f1f64-196">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="f1f64-196">The internal committed content version.</span></span> <span data-ttu-id="f1f64-197">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-197">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f1f64-198">fileName</span><span class="sxs-lookup"><span data-stu-id="f1f64-198">fileName</span></span>|<span data-ttu-id="f1f64-199">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-199">String</span></span>|<span data-ttu-id="f1f64-200">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="f1f64-200">The name of the main Lob application file.</span></span> <span data-ttu-id="f1f64-201">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-201">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f1f64-202">size</span><span class="sxs-lookup"><span data-stu-id="f1f64-202">size</span></span>|<span data-ttu-id="f1f64-203">Int64</span><span class="sxs-lookup"><span data-stu-id="f1f64-203">Int64</span></span>|<span data-ttu-id="f1f64-204">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="f1f64-204">The total size, including all uploaded files.</span></span> <span data-ttu-id="f1f64-205">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="f1f64-205">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="f1f64-206">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f1f64-206">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="f1f64-207">windowsMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="f1f64-207">windowsMinimumOperatingSystem</span></span>](../resources/intune-apps-windowsminimumoperatingsystem.md)|<span data-ttu-id="f1f64-208">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="f1f64-208">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="f1f64-209">productIdentifier</span><span class="sxs-lookup"><span data-stu-id="f1f64-209">productIdentifier</span></span>|<span data-ttu-id="f1f64-210">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-210">String</span></span>|<span data-ttu-id="f1f64-211">O identificador do produto.</span><span class="sxs-lookup"><span data-stu-id="f1f64-211">The Product Identifier.</span></span>|
|<span data-ttu-id="f1f64-212">identityVersion</span><span class="sxs-lookup"><span data-stu-id="f1f64-212">identityVersion</span></span>|<span data-ttu-id="f1f64-213">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f1f64-213">String</span></span>|<span data-ttu-id="f1f64-214">A versão da identidade.</span><span class="sxs-lookup"><span data-stu-id="f1f64-214">The identity version.</span></span>|



## <a name="response"></a><span data-ttu-id="f1f64-215">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f64-215">Response</span></span>
<span data-ttu-id="f1f64-216">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="f1f64-216">If successful, this method returns a `200 OK` response code and an updated [windowsPhoneXAP](../resources/intune-apps-windowsphonexap.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f1f64-217">Exemplo</span><span class="sxs-lookup"><span data-stu-id="f1f64-217">Example</span></span>
### <a name="request"></a><span data-ttu-id="f1f64-218">Solicitação</span><span class="sxs-lookup"><span data-stu-id="f1f64-218">Request</span></span>
<span data-ttu-id="f1f64-219">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="f1f64-219">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 1089

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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```

### <a name="response"></a><span data-ttu-id="f1f64-220">Resposta</span><span class="sxs-lookup"><span data-stu-id="f1f64-220">Response</span></span>
<span data-ttu-id="f1f64-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="f1f64-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1251

{
  "@odata.type": "#microsoft.graph.windowsPhoneXAP",
  "id": "301ddc77-dc77-301d-77dc-1d3077dc1d30",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.windowsMinimumOperatingSystem",
    "v8_0": true,
    "v8_1": true,
    "v10_0": true,
    "v10_1607": true,
    "v10_1703": true,
    "v10_1709": true,
    "v10_1803": true
  },
  "productIdentifier": "Product Identifier value",
  "identityVersion": "Identity Version value"
}
```





