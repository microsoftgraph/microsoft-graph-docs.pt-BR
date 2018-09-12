# <a name="deviceenrollmenttype-enum-type"></a>tipo enumerado deviceEnrollmentType

> **Importante:** as APIs na versão /beta no Microsoft Graph estão em versão prévia e estão sujeitas a alterações. Não há suporte para o uso dessas APIs em aplicativos de produção.

> **Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.

Maneiras possíveis de adicionar um dispositivo móvel ao gerenciamento.

## <a name="members"></a>Membros
|Membro|Valor|Descrição|
|:---|:---|:---|
|unknown|0|O valor padrão, tipo de registro não foi coletado.|
|userEnrollment|1|Inscrição do usuário direcionado por meio do canal BYOD.|
|deviceEnrollmentManager|2|Inscrição do usuário com uma conta de gerente de inscrição de dispositivo.|
|appleBulkWithUser|3|Inscrição da Apple em massa com o desafio de usuário (DEP, Apple Configurator).|
|appleBulkWithoutUser|4|Inscrição da Apple em massa sem o desafio de usuário (DEP, Apple Configurator, Mobile Config).|
|windowsAzureADJoin|5|Windows Azure AD 10 Join.|
|windowsBulkUserless|6|Inscrição em massa de Windows 10 por meio de ICD com certificado.|
|windowsAutoEnrollment|7|Inscrição automática do Windows 10. (Adicionar a conta de trabalho)|
|windowsBulkAzureDomainJoin|8|Windows 10 Azure AD Join em massa.|
|windowsCoManagement|9|Co-gerenciamento do Windows 10 é disparado pelo AutoPilot ou pela Diretiva de Grupo.|



