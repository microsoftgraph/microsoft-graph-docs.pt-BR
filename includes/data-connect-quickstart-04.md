---
ms.localizationpriority: medium
ms.openlocfilehash: 6297134d4f4de13bc2121772edf50e70ef12aa16
ms.sourcegitcommit: f99b4d365ba381f8f1997d3857ab43da03528924
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/13/2022
ms.locfileid: "66768187"
---
<!-- markdownlint-disable MD002 MD041 -->

Nesta etapa, você criará uma conta de Armazenamento do Azure em que a conexão de dados do Microsoft Graph armazenará os dados extraídos do Microsoft 365 para processamento adicional.

1. Abra um navegador e vá para o [Portal do Azure](https://portal.azure.com/).

1. Entre usando uma conta com direitos **Administrador global** seus locatários do Azure e do Microsoft 365.

1. Na barra lateral de navegação, selecione **Criar um recurso**.

1. Localize **o tipo de recurso** da Conta de Armazenamento e use os valores a seguir para criar e, em seguida, **selecione Examinar + criar**.

    - **Assinatura**: selecione sua assinatura do Azure
    - **Grupo de recursos**: GraphDataConnect (ou selecione um grupo de recursos existente)
    - **Nome da conta de** armazenamento: mgdcm365datastore
    - **Região**: escolha uma região do Azure na mesma região que a região do Microsoft 365
    - **Desempenho**: Padrão
    - **Redundância**: GRS (armazenamento com redundância geográfica)
    - **Guia Avançado**:
      - **Camada de acesso**: frequente

1. Examine se as configurações correspondem às mostradas na etapa anterior e selecione **Criar**.

1. Depois que a conta de Armazenamento do Azure tiver sido criada, conceda ao aplicativo Azure AD criado anteriormente o acesso adequado a ela.

    1. Selecione a **conta de Armazenamento do Azure**.
    2. No menu da barra lateral, selecione Controle **de acesso (IAM)**.
    3. Selecione o **botão Adicionar** no bloco **Adicionar uma atribuição de** função.
    4. Use os valores a seguir para localizar o aplicativo selecionado anteriormente para conceder a ele a função Colaborador de Dados do **Blob** de Armazenamento e, em seguida, **selecione Salvar**.

        - **Função**: Colaborador de Dados do Blob de Armazenamento
        - **Atribuir acesso a**: Usuário, grupo ou entidade de serviço
        - **Selecione**: Transferência de dados de conexão de dados do Microsoft Graph (o nome do Azure AD aplicativo criado anteriormente)

        ![Uma captura de tela mostrando a atribuição de função adequada ao aplicativo para o Microsoft Graph Data Connect na conta de Armazenamento do Azure no portal do Azure.](../concepts/images/data-connect-azure-storage-role.png)

1. Crie um novo contêiner na conta **mgdcm365datastore** do Armazenamento do Azure.

    1. Selecione a **conta mgdcm365datastore** do Armazenamento do Azure.
    2. No menu da barra lateral, selecione **Contêineres** na seção serviço **Blob** .
    3. Selecione o **botão +Contêiner** na parte superior da página, use os valores a seguir e, em seguida, **selecione Criar**.

        - **Nome**: m365mails
        - **Nível de acesso público**: privado (sem acesso anônimo)

        ![Uma captura de tela mostrando a criação de um novo contêiner chamado m365mails nos contêineres de blob da conta de armazenamento no portal do Azure.](../concepts/images/data-connect-azure-storage-container.png)
